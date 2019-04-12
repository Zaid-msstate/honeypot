Which Honeypot YOU deployed? 
- dionaea

Issues encountered:
- f1-micro was a real issue while working on this project...
It took me along time to figure out what is the problem.. 
gcloud compute instances create "mhn-honeypot-1" --machine-type "f1-micro" 
--subnet "default" --maintenance-policy "MIGRATE"  --scopes 
"https://www.googleapis.com/auth/devstorage.read_only",
"https://www.googleapis.com/auth/logging.write",
"https://www.googleapis.com/auth/monitoring.write",
"https://www.googleapis.com/auth/servicecontrol",
"https://www.googleapis.com/auth/service.management.readonly",
"https://www.googleapis.com/auth/trace.append" --tags "mhn-honeypot","http-server" --image
"ubuntu-1404-trusty-v20171010" --image-project "ubuntu-os-cloud" --boot-disk-size "10"
--boot-disk-type "pd-standard" --boot-disk-device-name "mhn-honeypot-1"\

Unresolved questions : 
- The longer the machine run, the more result of data collected

summary of data collected (attacks)
- dionaea (381) attacks

