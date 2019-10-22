# PANOSGraylogExtractor
Extractors for PAN-OS TRAFFIC, THREAT, SYSTEM and CONFIG syslog for Graylog

This is only extractor - it won't create a new input, dashboard or any other funkiness.

# Usage
Tested on Graylog 3.1.2

See https://myworldofit.net/?p=10958 for a screenshot version of this guide.

1. Download the relevant .json file from this repo for your PAN-OS version (only 8.1 and 9.0 supported at this time), open that JSON file up in Notepad (or similar) and copy the contents to clipboard.
2. On your Graylog web management console head to System / Inputs > Inputs.
3. From the list select the 'Manage extractors’ option next to your syslog input.
4. Click the Actions drop down and select ‘Import extractors’.
5. Paste the contents of the clipboard into the ‘Extractors JSON’ and click ‘Add extractors to input’.
6. Following the confirmation message head over to Streams, and select the stream that your PAN-OS syslog data is being captured in. From there you should now see any new data being parsed with the extractor.
