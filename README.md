# debezium-custom-masking-for-rdbms
Debezium maven custom data masking transformation for RDBMS databases

debezium server transformation settings:
```
debezium.transforms=MaskField
debezium.transforms.MaskField.type=com.nimin.medium.debezium.CustomMaskField$Value
debezium.transforms.MaskField.fields=email
```
# Steps to run
1. Build the jar:
```
mvn package
```
2. Copy the jar to lib folder of debezium server
3. Add the transformation settings in the debezium server application.properties file
4. Restart debezium server
