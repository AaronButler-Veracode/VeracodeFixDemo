# VeracodeFixDemo

# For latest instructions see: 
https://veracode-my.sharepoint.com/:w:/r/personal/cdalomba_veracode_com/Documents/!!Collaboration/VeracodeFixDemoFromRSA.docx?d=wdd1ad37ecef44318bab376b60c359a16&csf=1&web=1&e=zzHSLu

# Quick Demo
## Compile

javac -g SQLvulnerability.java

## Run SAST

veracode sast SQLvulnerability.class --emit-stack-dump --out results.json

## Run fix

veracode fix SQLvulnerability.java

## Recompile

javac -g SQLvulnerability.java

## Run SAST on new class file

veracode sast SQLvulnerability.class --emit-stack-dump --out results.json

## Reset the demo (restore the source file)

cp SQLvulnerability.java.backup SQLvulnerability.java
