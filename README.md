# An Easy To Use Arduino Library Template

So you found this library template, cool! This is based off of how Adafruit makes their Arduino libraries. There are a few things that we need to update before you're ready to deploy!

### Steps to use this template ###

**FIRST**
<br>
The first thing you want to do is update the name of the `hello.h` and `hello.cpp` files. These will be your main CPP files for your Arduino library. They should match a structure to give an idea of what it does. 

If you are making a sensor library for instance, you will want it to be like `sensor_name.h` and `sensor_name.cpp`. 

If you are implementing some kind fo protocol or helper library, it shouild be like 'protocol_name.h` and `protocol_name.cpp`.

The example in the `examples` directory should also have it's named changed to match your top level class name.

**SeECOND** <br>

You will need to update the `library.properties` file to include your repo name, your name, maintainer, project name, etc...

**THIRD**<br>

You will need to update the `githubci.yml` file in `.github/workflows/` directory. You need to make sure you include any other libraries you are using. It's highly recommended to use Adafruit helper libraries because this template is based off how Adafruit builds their libraries.

**FINALLY**<br>

You will need to update the CMakeLists.txt to include any and all CPP files you want built for ESP-IDF related boards. If you don't do this, there's no guarantee they will work or build for ESP-IDF dependent devices.

### Troubleshooting ###

If you have any problems using this template, please use the discussions tab or file an issue.

### Contributing ###

Please reference the adafruit contributing guidelines and code of conduct for a general guidance of what is expected from contributors. This template is not sponsored by or used by Adafruit directly, and there is no affiliation other than it being based on the way Adafruit deploys Arduino libraries. 
