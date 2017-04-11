# Explorer Kit Hardware Abstraction Layer

Use the ExplorerKit_001 and ExplorerKit_004m tables to access the hardware pins, i2c sensor addresses, i2c and spi bus objects.

## ExplorerKit_001

* LED_SPI
* SENSOR_AND_GROVE_I2C
* TEMP_HUMID_I2C_ADDR
* ACCEL_I2C_ADDR
* PRESSURE_I2C_ADDR
* POWER_GATE_AND_WAKE_PIN
* AD_GROVE1_DATA1
* AD_GROVE2_DATA1

### Example:

```
ExplorerKit_001.SENSOR_AND_GROVE_I2C.configure(CLOCK_SPEED_400_KHZ);
tempHumid <- HTS221(ExplorerKit_001.SENSOR_AND_GROVE_I2C, ExplorerKit_001.TEMP_HUMID_I2C_ADDR);
```

## ExplorerKit_004m

* LED_SPI
* SENSOR_I2C
* GROVE_I2C
* TEMP_HUMID_I2C_ADDR
* ACCEL_I2C_ADDR
* PRESSURE_I2C_ADDR
* POWER_GATE
* WAKE_PIN
* ACCEL_INT_PIN
* PRESSURE_INT_PIN
* AD_GROVE1_DATA1
* AD_GROVE1_DATA2
* AD_GROVE2_DATA1
* AD_GROVE2_DATA2

### Example:

```
ExplorerKit_004m.SENSOR_I2C.configure(CLOCK_SPEED_400_KHZ);
tempHumid <- HTS221(ExplorerKit_004m.SENSOR_I2C, ExplorerKit_004m.TEMP_HUMID_I2C_ADDR);
```

## License

Explorer Kit Hardware Abstraction Layer is licensed under the [MIT License](/LICENSE).