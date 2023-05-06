# Apple M1 temp sensor

## Why ?
I was frustrated by "Temperature: Not detected" in https://github.com/HorlogeSkynet/archey4 output.


## How to use ?

```shell
git clone https://github.com/delneg/apple-m1-temp-sensor-objc.git
cd apple-m1-temp-sensor-objc
make build
ln -s ~/.local/bin/temp_sensor ~/.local/bin/osx-cpu-temp
archey -j | jq ."data"."Temperature"
#{
#  "temperature": 41.2,
#  "max_temperature": 41.2,
#  "char_before_unit": " ",
#  "unit": "C"
#}
```
