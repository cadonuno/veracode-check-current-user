# Veracode Check Current User

## Overview

This script can be used to verify your user permissions and team membership

## Installation

Clone this repository:

    git clone https://github.com/cadonuno/veracode-check-current-user.git

Install dependencies:

    cd veracode-check-current-user
    pip install -r requirements.txt

### Getting Started

It is highly recommended that you store veracode API credentials on disk, in a secure file that has 
appropriate file protections in place.

(Optional) Save Veracode API credentials in `~/.veracode/credentials`

    [default]
    veracode_api_key_id = <YOUR_API_KEY_ID>
    veracode_api_key_secret = <YOUR_API_KEY_SECRET>

    
### Running the script
    py user_permissions.py [-d]
        You can pass -d to get verbose output for the API call

If a credentials file is not created, you can export the following environment variables:

    export VERACODE_API_KEY_ID=<YOUR_API_KEY_ID>
    export VERACODE_API_KEY_SECRET=<YOUR_API_KEY_SECRET>
    python user_permissions.py [-d]

## License

[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

See the [LICENSE](LICENSE) file for details
