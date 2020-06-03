Intelligent Customer Help Desk with Smart Document Understanding

This repository contains the project report and the Node-Red flow of the chatbot developed for Ecobee3 thermostat using various IBM Cloud Services.

The typical customer care chatbot can answer simple questions, such as store locations and hours, directions, and maybe even making appointments. When a question falls outside of the scope of the pre-determined question set, the option is typically to tell the customer the question isn’t valid or offer to speak to a real person.

In this project, if the customers' question is about the operation of a device, the application shall pass the question onto Watson Discovery Service, which has been pre-loaded with the device’s owners manual and shall return relevant sections of the owners manual to help solve our customers’ problem. The chatbot shall try to resolve all of the customers' queries untill the customer asks to speak to a representative.

To take it a step further, the Smart Document Understanding feature of Watson Discovery is used to train the Watson Discovery service as to what text in the owners manual (ecobee3_userguide) is important. This improves the answers returned by the Watson Discovery service. Then using IBM cloud functions action as webhook, Watson Discovery is integrated with Watson Assistant. Finally using Node-Red, Watson assistant is integrated with a web UI. This UI is then used to connect with Watson Assistant and chat with it.

Node-Red Dashboard link after deploying : https://ilicit.eu-gb.mybluemix.net/ui

