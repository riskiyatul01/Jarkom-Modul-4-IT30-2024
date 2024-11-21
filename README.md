# Jarkom-Modul-2-IT30-2024

**KELOMPOK IT30**
| Nama | NRP |
|---------------------------|------------|
|Riskiyatul Nur Oktarani | 5027231013 |
|Malvin Putra Rismahardian | 5027231048 |


# Hololive (Gateway)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp

# A1 > HoloID
auto eth1
iface eth1 inet static
    address 192.248.19.73
    netmask 255.255.255.252

# A8 > HoloJP
auto eth2
iface eth2 inet static
    address 192.248.19.105
    netmask 255.255.255.252

# A15 > HoloEN
auto eth3
iface eth3 inet static
    address 192.248.19.81
    netmask 255.255.255.252
HoloID
# A1 > Hololive
auto eth0
iface eth0 inet static
    address 192.248.19.74
    netmask 255.255.255.252
    gateway 192.248.19.73

# A2 > Holoro
auto eth1
iface eth1 inet static
    address 192.248.19.97
    netmask 255.255.255.252

# A4 > Area15
auto eth2
iface eth2 inet static
    address 192.248.19.93
    netmask 255.255.255.252

# A6 > Holoh3ro
auto eth3
iface eth3 inet static
    address 192.248.19.100
    netmask 255.255.255.252
Holoro
# A2 > HoloID
auto eth0
iface eth0 inet static
    address 192.248.19.94
    netmask 255.255.255.252
    gateway 192.248.19.93

# A3 > Switch7 > Ollie / Anya / Reine
auto eth1
iface eth1 inet static
    address 192.248.18.193
    netmask 255.255.255.192
```

Ollie
```
# A3 > Holoro
auto eth0
iface eth0 inet static
    address 192.248.18.194
    netmask 255.255.255.192
    gateway 192.248.18.193
```

Anya
```
# A3 > Holoro
auto eth0
iface eth0 inet static
    address 192.248.18.195
    netmask 255.255.255.192
    gateway 192.248.18.193
```

Reine
```
# A3 > Holoro
auto eth0
iface eth0 inet static
    address 192.248.18.196
    netmask 255.255.255.192
    gateway 192.248.18.193
```

# Area15
```
# A4 > HoloID
auto eth0
iface eth0 inet static
    address 192.248.19.93
    netmask 255.255.255.252
    gateway 192.248.19.92

# A5 > Switch6 > Moona / Risu / Iofi
auto eth1
iface eth1 inet static
    address 192.248.18.1
    netmask 255.255.252.0
```

Moona
```
# A5 > Area15
auto eth0
iface eth0 inet static
    address 192.248.18.2
    netmask 255.255.252.0
    gateway 192.248.18.1
```

Risu
```
# A5 > Area15
auto eth0
iface eth0 inet static
    address 192.248.18.3
    netmask 255.255.252.0
    gateway 192.248.18.1
```

Iofi
```
# A5 > Area15
auto eth0
iface eth0 inet static
    address 192.248.18.4
    netmask 255.255.252.0
    gateway 192.248.18.1
```

# Holoh3ro
```
# A6 > HoloID
auto eth0
iface eth0 inet static
    address 192.248.19.101
    netmask 255.255.255.252
    gateway 192.248.19.100

# A7 > Switch8 > Zeta / Kaela / Kobo
auto eth1
iface eth1 inet static
    address 192.248.16.1
    netmask 255.255.254.0
```

Zeta
```
# A7 > Holoh3ro
auto eth0
iface eth0 inet static
    address 192.248.16.2
    netmask 255.255.254.0
    gateway 192.248.16.1
```

Kaela
```
# A7 > Holoh3ro
auto eth0
iface eth0 inet static
    address 192.248.16.3
    netmask 255.255.254.0
    gateway 192.248.16.1
```

Kobo
```
# A7 > Holoh3ro
auto eth0
iface eth0 inet static
    address 192.248.16.4
    netmask 255.255.254.0
    gateway 192.248.16.1
```

# HoloJP
```
# A8 > Hololive
auto eth0
iface eth0 inet static
    address 192.248.19.106
    netmask 255.255.255.252
    gateway 192.248.19.105

# A9 > Switch1 > DEV_IS / GEN:0
auto eth1
iface eth1 inet static
    address 192.248.19.64
    netmask 255.255.255.248
```

# DEV_IS
```
# A9 > HoloJP
auto eth0
iface eth0 inet static
    address 192.248.19.65
    netmask 255.255.255.248
    gateway 192.248.19.64

# A10 > Switch2 > Re:Gloss > Ririka_Raden / Ao / Hajime_Kanade
auto eth1
iface eth1 inet static
    address 192.248.19.33
    netmask 255.255.255.240
```

Ririka_Raden
```
# A10 > DEV_IS
auto eth0
iface eth0 inet static
    address 192.248.19.34
    netmask 255.255.255.240
    gateway 192.248.19.33
```

Ao
```
# A10 > DEV_IS
auto eth0
iface eth0 inet static
    address 192.248.19.35
    netmask 255.255.255.240
    gateway 192.248.19.33
```

Hajime_Kanade
```
# A10 > DEV_IS
auto eth0
iface eth0 inet static
    address 192.248.19.36
    netmask 255.255.255.240
    gateway 192.248.19.33
```

# GEN:0
```
# A9 > HoloJP
auto eth0
iface eth0 inet static
    address 192.248.19.67
    netmask 255.255.255.248
    gateway 192.248.19.64

# A11 > Switch3 > MiComet / Sora_Robo_AZK / GEN:1
auto eth1
iface eth1 inet static
    address 192.248.0.1
    netmask 255.255.248.0
```

MiComet
```
# A11 > GEN:0
auto eth0
iface eth0 inet static
    address 192.248.0.2
    netmask 255.255.248.0
    gateway 192.248.0.1
```

Sora_Robo_AZK
```
# A11 > GEN:0
auto eth0
iface eth0 inet static
    address 192.248.5.224
    netmask 255.255.248.0
    gateway 192.248.0.1
```

# GEN:1
```
# A11 > GEN:0
auto eth0
iface eth0 inet static
    address 192.248.0.3
    netmask 255.255.248.0
    gateway 192.248.0.1

# A12 > Switch4 > FBKK_Matsuri / Aki_Haachama
auto eth1
iface eth1 inet static
    address 192.248.14.1
    netmask 255.255.254.0

# A13 > Switch5 > GAMERS
auto eth2
iface eth2 inet static
    address 192.248.19.77
    netmask 255.255.255.252
```

FBK_Matsuri
```
# A12 > Switch Member
auto eth0
iface eth0 inet static
    address 192.248.14.2
    netmask 255.255.254.0
    gateway 192.248.14.1
```

Aki_Hachama
```
# A12 > Switch Member
auto eth0
iface eth0 inet static
    address 192.248.14.3
    netmask 255.255.254.0
    gateway 192.248.14.1
```

# GAMERS
```
# A13 > GEN:1
auto eth0
iface eth0 inet static
    address 192.248.19.77
    netmask 255.255.255.252
    gateway 192.248.19.76

# A14 > Fubuki / Korone / Okayu / Mio
auto eth1
iface eth1 inet static
    address 192.248.18.1
    netmask 255.255.255.128
```

Korone
```
# A14 > GAMERS
auto eth0
iface eth0 inet static
    address 192.248.18.2
    netmask 255.255.255.128
    gateway 192.248.18.1
```

Okayu
```
# A14 > GAMERS
auto eth0
iface eth0 inet static
    address 192.248.18.3
    netmask 255.255.255.128
    gateway 192.248.18.1
```

Mio
```
# A14 > GAMERS
auto eth0
iface eth0 inet static
    address 192.248.18.4
    netmask 255.255.255.128
    gateway 192.248.18.1
```

# HoloEN
```
# A15 > Hololive
auto eth0
iface eth0 inet static
    address 192.248.19.82
    netmask 255.255.255.252
    gateway 192.248.19.81

# A16 > HoloAdvent
auto eth1
iface eth1 inet static
    address 192.248.19.85
    netmask 255.255.255.252

# A18 > HoloMyth
auto eth2
iface eth2 inet static
    address 192.248.19.88
    netmask 255.255.255.252
```

# HoloAdvent
```
# A16 > HoloEN
auto eth0
iface eth0 inet static
    address 192.248.19.86
    netmask 255.255.255.252
    gateway 192.248.19.85

# A17 > Switch5 > FuwaMoco / Shiori_Nerissa / Biboo
auto eth1
iface eth1 inet static
    address 192.248.19.1
    netmask 255.255.255.224
```

FuwaMoco
```
# A17 > HoloAdvent
auto eth0
iface eth0 inet static
    address 192.248.19.2
    netmask 255.255.255.224
    gateway 192.248.19.1
```

Shiori_Nerissa
```
# A17 > HoloAdvent
auto eth0
iface eth0 inet static
    address 192.248.19.7
    netmask 255.255.255.224
    gateway 192.248.19.1
```

Biboo
```
# A17 > HoloAdvent
auto eth0
iface eth0 inet static
    address 192.248.19.18
    netmask 255.255.255.224
    gateway 192.248.19.1
```

# HoloMyth
```
# A18 > HoloEN
auto eth0
iface eth0 inet static
    address 192.248.19.89
    netmask 255.255.255.252
    gateway 192.248.19.88

# A19 > Switch2 > Gura_Ame_Ina / Kiara_Calli
auto eth1
iface eth1 inet static
    address 192.248.12.1
    netmask 255.255.254.0

# A20 > Project-Hope / Holo-Council
auto eth2
iface eth2 inet static
    address 192.248.19.49
    netmask 255.255.255.248
```

Gura_Ame_Ina
```
# A19 > HoloMyth
auto eth0
iface eth0 inet static
    address 192.248.12.2
    netmask 255.255.254.0
    gateway 192.248.12.1
```

Kiara_Calli
```
# A19 > HoloMyth
auto eth0
iface eth0 inet static
    address 192.248.13.55
    netmask 255.255.254.0
    gateway 192.248.12.1
```

# Project-Hope
```
# A20 > HoloMyth
auto eth0
iface eth0 inet static
    address 192.248.19.50
    netmask 255.255.255.248
    gateway 192.248.19.49

# A21 > Switch7 > Irys
auto eth1
iface eth1 inet static
    address 192.248.19.57
    netmask 255.255.255.248
```

Irys
```
# A21 > Project-Hope
auto eth0
iface eth0 inet static
    address 192.248.19.58
    netmask 255.255.255.248
    gateway 192.248.19.57
```

# HoloCouncil
```
# A20 > Project-Hope
auto eth0
iface eth0 inet static
    address 192.248.19.51
    netmask 255.255.255.248
    gateway 192.248.19.49

# A20 > HoloMyth
auto eth1
iface eth1 inet static
    address 192.248.19.53
    netmask 255.255.255.248
    gateway 192.248.19.52

# A22 > Switch4 > Kronii_Mumei / Bae_Fauna
auto eth2
iface eth2 inet static
    address 192.248.18.129
    netmask 255.255.255.192
```

Kronii_Mumei
```
# A22 > HoloCouncil
auto eth0
iface eth0 inet static
    address 192.248.18.130
    netmask 255.255.255.192
    gateway 192.248.18.129
```

Bae_Fauna
```
# A22 > HoloCouncil
auto eth0
iface eth0 inet static
    address 192.248.18.168
    netmask 255.255.255.192
    gateway 192.248.18.129
```
