# Install PHPMD
## How to global install PHPMD with Composer

    composer global require phpmd/phpmd
    
## Copy this rulesets into global phpmd folder
### Replace all xml ruleset file into phpmd\phpmd\src\main\resources\rulesets.
    git clone git@github.com:AurelienMo/tools-phpmd.git
    cp /PATH/TO/tools-phpmd /PATH/TO/GLOBALINSTALLPHP/phpmd/phpmd/src/main/resources/rulesets
    
- Example on Windows:

    
    cp C:\Users\amor\Downloads\tools-phpmd\* C:\Users\amor\AppData\Roaming\Composer\vendor\phpmd\phpmd\src\main\resources\rulesets


## Launch PHPMD withou git hooks pre-commit:
        
        phpmd sourceDirectory output path/to/ruleset/phpmd_symfony.xml
        
**sourceDirectory:** Filename or directory to analyze

**output:** Output type for this command:
- text, html or xml

**path/to/ruleset/phpmd_symfony.xml**: Path to phpmd_symfony.xml file on your computer
