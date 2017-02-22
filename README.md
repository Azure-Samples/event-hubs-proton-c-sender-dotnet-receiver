The hello_world sample sends 200 messages to an Event Hub.

Follow the instructions here to build and install Proton.
https://git-wip-us.apache.org/repos/asf?p=qpid-proton.git;a=blob;f=INSTALL.md;hb=0.17.0

Build the sample (modify the compiler options based on your config).
g++ -L/usr/lib64 -lqpid-proton-cpp -o sender helloworld.cpp

Run the sameple.
./sender amqps://SASKeyName:SASKey@YourNamespace.servicebus.windows.net/YourEventHub

Replace SASKeyName, SASKey, YourNamespace and YourEventHub with the values from your setup.

Note that SASKeyName and SASKey need to be URL encoded.

This example was based on the Proton C++ sample.
https://qpid.apache.org/releases/qpid-proton-0.17.0/proton/cpp/examples/helloworld.cpp.html

# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
