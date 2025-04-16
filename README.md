# VeracodeFixDemo

## For latest instructions see: 
https://veracode-my.sharepoint.com/:w:/p/cdalomba/EX7TGt30zhhDurN2tgw1mhYB8hJwVDDkSIZ77lzLYOi1qg?e=sxNhq8

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

Change 1
