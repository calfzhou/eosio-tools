# eosio-tools

## eos convert

Use `./eos_convert.py --help` for usage.

Examples:

``` bash
$ ./eos_convert.py name encode eosio.token
6138663591592764928
$ ./eos_convert.py name encode --hex eosio.token
0x5530ea033482a600
$ ./eos_convert.py name encode --hex --little eosio.token
0x00a6823403ea3055

$ ./eos_convert.py name decode 6138663591592764928
eosio.token
$ ./eos_convert.py name decode --hex 0x5530ea033482a600
eosio.token
$ ./eos_convert.py name decode --hex --little 0x00a6823403ea3055
eosio.token

$ ./eos_convert.py symbol encode 4,EOS
1397703940
$ ./eos_convert.py symbol encode --hex 4,EOS
0x00000000534f4504
$ ./eos_convert.py symbol encode --hex --little 4,EOS
0x04454f5300000000

$ ./eos_convert.py symbol decode 1397703940
4,EOS
$ ./eos_convert.py symbol decode --hex 0x00000000534f4504
4,EOS
$ ./eos_convert.py symbol decode --hex --little 0x04454f5300000000
4,EOS
```

C++ demo: [https://ideone.com/OLNVKJ](https://ideone.com/OLNVKJ)
