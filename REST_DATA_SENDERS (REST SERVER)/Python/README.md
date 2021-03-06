# PI-Connector-for-UFL-Samples - PYTHON

These samples show how to get started with the PI Connector for UFL REST endpoint feature.

## Contents

* Python samples to create a data file and then use the a HTTP Put command to send the data file to the UFL REST endpoint.

## Getting Started

You will need a development/test PI System and the PI Connector for UFL (the samples were tested with version 1.0.0.41).
The scripts to send data have been tested with Pyhon 3.5.1 and come in two versions. 
* piuflput.py - uses the Python requests module. The request module simplifies a lot the sending and receiving of http requests and it is strongly encouraged to use this module. 
* piuflput_urllib.py - uses only Python modules that are part of a standard install of Python3.

## Tutorial on how to use these scripts
1. Open the PI Connector for UFL admin page by opening a browser and visiting: [https://{servername}:{port}/admin/ui/](https://{servername}:{port}/admin/ui/).
2. Specify a PI Data Archive and create a new data source.
3. Upload value.ini as the Config File and select a username and password.
4. Make the following choices:
    * Select Rest as the Data Source Type
    * Leave New Line as blank
    * Select UTC for Incoming TimeStamps
5. Save the data source and reopen it. The address field will now be populated.
6. Copy the url in the address field and navigate to the folder where the Python sample code is stored.
7. Run the command below to send data.

    `python piuflput_urllib.py url value.csv`

    `python piuflgen.py value > morevalues.csv`

##Licensing

Copyright 2016 OSIsoft, LLC.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
   
Please see the file named [LICENSE.md](LICENSE.md).

