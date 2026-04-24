# API_2026
### Your Flow
1) Create new user
    - verify that response code is equal to 201
    - verify that role is equal to "user"
    - check that apiKey is available and not empty
    - store apiKey in collection variable
2) Verify that balance on user's account is 100 000 Czechitokens
    - verify that response code is equal to 200
    - verify that account balance is 100000
    - store account nr. in collection variable (e.g. initialAccNr)
    - store account id in collection variable  (e.g. initialAccId)
3) Create new account for that user
    - verify that response code is equal to 201
    - verify that account was successfully created (=true)
    - verify that account balance is 0
    - store account nr. in collection variable (e.g. newAccNr)
    - store account id in collection variable  (e.g. newAccId)
4) Rename that account
    - verify that response code is equal to 200
    - verify that account was successfully renamed (success=true)    
5) Send 100 Czechitokens from default account to newly created one
    - verify that response code is equal to 201
    - verify that transaction was successfully created (success=true)
6) Verify that new balance on default account is 99 900
    - verify that response code is equal to 200
    - verify that new account balance is 99 900
7) Verify that new balance on newly created account is 100
    - verify that response code is equal to 200
    - verify that account balance is 100
