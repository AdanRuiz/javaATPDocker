# Standalone Notes

Java ATP Docker example

## Setup ATP DB

1. Create user TODOUSER with DATA unlimited restriction 
2. Create table:
CREATE TABLE TODOUSER.sometable (id NUMBER GENERATED ALWAYS AS IDENTITY, description VARCHAR2(4000), creation_ts TIMESTAMP WITH TIME ZONE DEFAULT CURRENT_TIMESTAMP, done NUMBER(1,0) , PRIMARY KEY (id));
3. Identify TNS Name
4. Download Wallet

## App setup
1. Download/Clone project
2. Modify application.properties (src/main/resources):
    - TNS Name
    - Wallet PATH
    - Password
3. mvn verify
4. java -jar  target/Micros...jar
5. Test locally: http://localhost:9898/function