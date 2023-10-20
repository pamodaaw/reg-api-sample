Scenario 1:
-----------

* enable auto login
* add the user to the default userstore.
* steps:
    1. Onboard password | Continue with email OTP
    2. Verify email address
* script:
    execute step 1
    Once step 1 is completed
        if selected option is password
            execute step 2
    Complete

Scenario 2:
------------

* enable auto login
* add the user to the "ABC" user store.
* steps 
    1. Onboard password
    2. Verify email address
    3. Collect the country, city and postal code
    4. Collect the passport number
    5. Collect the NIC
    6. Verify mobile number
* script
    execute step 1
    execute step 2
    execute step 3
    Once step 3 is completed
        if residence of SL
            execute step 5
        else 
            execute step 4
    Execute step 6
    Complete

 <!-- 
 Scenario 2:
------------

* enable auto login
* add the user to the default user store.
* steps 
    1. Onboard password
    2. Verify email address
    3. Collect the country, _If non-residence of SL, execute step 4, otherwise execute step 5_
    4. Collect the passport number
    5. Collect the NIC 
    -->
