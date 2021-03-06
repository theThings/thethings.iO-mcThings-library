# thethingsiO-mcThings-library

This repository contains all the necessary data to connect the mcGateway <img src="https://static1.squarespace.com/static/5644f11fe4b0d6ca7d80d351/56464858e4b0a4a3eeee164f/571fa990f8baf3aa08ceba95/1461692818210/mc-gateway.jpg" alt="Drawing" width="200"/>  and mcModule 120  <img src="https://static1.squarespace.com/static/5644f11fe4b0d6ca7d80d351/56464858e4b0a4a3eeee164f/5772e7cdebbd1ab65ac0481d/1486135599593/mc-mod120.jpg" alt="Drawing" width="200"/> (from mcThings) to 
thethings.iO.

The project extracts both the ambient temperature (from the temperature sensor, in ºC) and the battery level (in miliVolts) and sends them every 10 and 30 seconds using the thethingsiO provided library.

In order to upload this project in your device, follow this steps:

0. Download and install mcStudio from mcthings. Make sure you have installed the latest .Net Framework (4.6.2).

1. Download this repository and place it in the mcThings folder, along with your other projects and libraries (inisde My Documents).

2. Open this project with the mcStudio

3. Create an account, a product and generate the first thing in thethings.iO platform. If you already have an account, make you you have unused activationCodes or free thingTokens.

4. Copy the thingToken of the previous activated product and paste it to the token variable in the Project code (Temp.mcScript)

```
Shared Event Boot()
    token = "YOURTHINGTOKEN"
```

5. Configure your mcGateway mqtt options:

<img src="http://blog.thethings.io/wp-content/uploads/2017/02/thethings-gateway-config-1.png" alt="Drawing"/>

6. Deploy the code to your mcModule.

