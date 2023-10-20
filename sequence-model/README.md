This folder contains object definitions and samples for the registration sequence.

[Object Definition](definition.json)

## Samples

### Scenario 1:  

* enable auto login
* add the user to the default userstore.
* step definitions: <br>
    - Step A. Onboard password | Continue with email OTP <br>
    - Step B. Verify email address <br>
* flow defintion:
```
    Start
    Execute step A
    When step A is completed
        if selected option is Password
            execute step B
    Complete
```

![Alt text](reference-images/image-1.png)

[Sample Object definition](sample1.json)

### Scenario 2:

* enable auto login
* add the user to the "ABC" user store.
* step definitions: <br>
    - Step 1. Onboard password <br>
    - Step 2. Verify email address <br>
    - Step 3. Collect the country, city and postal code <br>
    - Step 4. Collect the passport number <br>
    - Step 5. Collect the NIC <br>
    - Step 6. Verify mobile number <br>
* flow defintion:
```
    Start
    Execute step 1
    Execute step 2
    Execute step 3
    When step 3 is completed
        if residence of SL
            execute step 5
        else 
            execute step 4
    Execute step 6
    Complete
```

![Alt text](reference-images/image.png)

[Sample Object Definition](sample2.json)


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
