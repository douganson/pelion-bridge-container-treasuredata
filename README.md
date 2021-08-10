arm PELION Device Shadow bridge for TreasureData Observation Telemetry
  
08/09/2021: updated bridge - better support for unified formatting of notifications/responses

08/08/2021: updated bridge - minor fixes and updates for AWS and Pelion

01/07/2021: updated bridge - minor fixes and dependency updates

08/31/2020: updated bridge - updated dependencies

02/29/2020: updated bridge - fixes for draft mode MQTT (token handling) 

02/29/2020: updated bridge - updated for treasuredata support. minor marshalling fixes

02/26/2020: initial checkin

Container Bridge Instance Installation:

1). Clone this repo into a Linux instance that supports docker

2). cd into the cloned repo and run: ./run-reload-bridge.sh

3). Next go to https://os.mbed.com and create your mbed Account. You can then request a Pelion developer account using the same credentials at https://portal.us-east-1.mbedcloud.com

4). Acquire a TreasureData account and create a Master Key API token

4). Once your Pelion account is created, you need to "Access Keys" to create a Pelion API Key/Token. Record the Token Value

Now that you have your:

    - TreasureData Master API Key

    - Pelion API Key/Token generated

Go to:  https://[[your containers public IP address]]:8234

    - username: "admin" (no quotes)

    - password: "admin" (no quotes)

Enter your TreasureData Master API Key and Pelion API Token

    - Please press "SAVE" after *each* is entered... 

    - After all are entered and saved, press "RESTART"

Your TreasureData bridge should now be configured and operational. 

Bridge source (Apache 2.0 licensed - Enjoy!): https://github.com/ARMmbed/pelion-bridge.git

Copyright 2020. ARM Ltd. All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License. 
