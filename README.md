# sigma-tactics-organizer
Script that organize Sigma rules by MITRE | ATT&amp;CK tactics and techniques. 

Download the Sigma rules from the awesome public project SigmaHQ (https://github.com/SigmaHQ/sigma/tree/master/rules) then with this simple script you will have all the rules organized in 2 main folders (`tactics` and `techniques`) and many sub-folders for different typology.
```
mitre
  --> tactics
          --> TA0043_reconnaissance
          --> TA0042_resource_development
          --> ...
  --> techniques
          --> T1002
          --> T1006
          --> ...
```

The script considers as input path `../sigma/rules/` and as the output path `/sigma/rules/mitre`. This can be easily modified by changing the following lines of the scripts 

`root_directory = script_directory+'/sigma/rules/windows'`  
`destination_base_directory = script_directory+'/sigma/rules/mitre'`


## Example
from shell:
```bash
$ python3 RulesMitreOrganizer.py
```

## References
https://raw.githubusercontent.com/mitre/cti/master/enterprise-attack/enterprise-attack.json

https://github.com/SigmaHQ/sigma
