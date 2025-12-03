# n8n-passive-subdomain-enumeration
This n8n workflow performs passive subdomain enumeration and uses an AI-powered filter to highlight only the subdomains that appear sensitive or interesting, such as admin, dev, or staging environments. It outputs a clean, relevant list for use in recon, bug bounty work, and security automation.


## Setup

1. Set your SSH credentials
2. Install required tools : subfinder, assetfinder, httpx, httpx-toolkit
3. I used perplexity Ai , you can use any you want setup and add API of your model

## Run

1. start workflow
2. upload the domain list to webhook by url in webhook with curl with domain text file
3. example : curl -X POST -F "file=@domain.txt" http://localhost:5678/webhook-test/upload-file
