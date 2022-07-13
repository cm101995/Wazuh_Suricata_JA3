# Wazuh_Suricata_JA3

This code helps in comparing the JA3 hashes against the malicious ones from abuse.ch website. 

Prerequisites:
1)Suricata logs are being sent to Wazuh
2)Have malicious JA3 hashes locally within Wazuh directory

1) Download the malicious hashes locally (https://sslbl.abuse.ch/blacklist/ja3_fingerprints.csv)
2) Create a custom active response rule in Wazuh.

ja3.txt is the file downloaded from abuse.ch(cron job to download it daily). This has a list of malicious JA3 hashes.
suricata.json is an example of TLS related events in suricata. We extract JA3 field from the log and compare it against the ja3.txt file.

Reference:
1)https://documentation.wazuh.com/current/user-manual/capabilities/active-response/custom-active-response.html
2)https://abuse.ch/
