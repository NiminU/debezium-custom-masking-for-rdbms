# debezium-custom-masking-for-rdbms
Debezium maven custom data masking transformation for RDBMS databases

debezium server transformation settings:
```
debezium.transforms=MaskField
debezium.transforms.MaskField.type=com.nimin.medium.debezium.CustomMaskField$Value
debezium.transforms.MaskField.fields=email
```
