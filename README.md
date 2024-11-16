# Jarkom-Modul-4-IT07-2024

Kelompok IT07:

- Dimas Andhika Diputra 5027231074
- Kharisma Fahrun Nisa 5027231086

# Topologi

<img src="./img/topo-cpt-modul4.png" />

# Rute

| Nama Subnet | Rute                                                                                                                                                  |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| A1          | Hololive > Holo-EN                                                                                                                                    |
| A2          | Hololive > Holo-EN > HoloAdvent                                                                                                                       |
| A3          | Hololive > Holo-EN > Holo-Myth                                                                                                                        |
| A4          | Hololive > Holo-EN > Holo-Myth > Switch2 > Gura_Aine_Ina (309 Host) > Switch2 > Kiara_Calli (193 Host)                                                |
| A5          | Hololive > Holo-EN > HoloAdvent > Switch0 > FuwaMoco (5 Host) > Switch0 > Shiori_Nerissa (12 Host) > Switch0 > Biboo (10 Host)                        |
| A6          | Hololive > Holo-EN > Holo-Myth > HoloPromise > Router4 > HoloPromise > Holo-Council                                                                   |
| A7          | Hololive > Holo-EN > Holo-Myth > HoloPromise > Router4 > Tys (2 Host)                                                                                 |
| A8          | Hololive > Holo-EN > Holo-Myth > HoloPromise > Holo-Council > Switch4 > Kronii_Mumei (39 Host) > Switch4 > Bae_Fauna (22 Host)                        |
| A9          | Hololive > Holo-JP                                                                                                                                    |
| A10         | Hololive > Holo-JP > Switch1 > DEV_IS > Switch1 > GEN:0                                                                                               |
| A11         | Hololive > Holo-JP > Switch1 > DEV_IS > `Re:GLO$$` > Ririka_Raden (3 Host) > `Re:GLO$$` > Ao (3 Host) > `Re:GLO$$` > Hajime_Kanade (7 Host)           |
| A12         | Hololive > Holo-JP > Switch1 > GEN:0 > Switch3 > MiComet (1501 Host) > Switch3 > Sora_Robo_AZKi (542 Host) > Switch3 > GEN:1                          |
| A13         | Hololive > Holo-JP > Switch1 > GEN:0 > Switch3 > GEN:1 > GAMERS                                                                                       |
| A14         | Hololive > Holo-JP > Switch1 > GEN:0 > Switch3 > GEN:1 > GAMERS > Switch13 > Korone (51 Host) > Switch13 > Okayu (32 Host) > Switch13 > Mio (36 Host) |
| A15         | Hololive > Holo-JP > Switch1 > GEN:0 > Switch3 > GEN:1 > Member > FBK_Matsuri (342 Host) > Member > Aki_Hachama (148 Host)                            |
| A16         | Hololive > Holo-ID                                                                                                                                    |
| A17         | Hololive > Holo-ID > AREA15                                                                                                                           |
| A18         | Hololive > Holo-ID > AREA15 > Switch6 > lofi (140 Host) > Switch6 > Risu (319 Host) > Switch6 > Moona (201 Host)                                      |
| A19         | Hololive > Holo-ID > holoro                                                                                                                           |
| A20         | Hololive > Holo-ID > holoh3ro                                                                                                                         |
| A21         | Hololive > Holo-ID > holoh3ro > Switch8 > Zeta (81 Host) > Switch8 > Kaela (71 Host) > Switch8 > Kobo (146 Host)                                      |
| A22         | Hololive > Holo-ID > holoro > Switch7 > Ollie (20 Host) > Switch7 > Anya (3 Host) > Switch7 > Reine (10 Host))                                        |

# Area Subnet

| Nama Subnet | Area Subnet                                                                           | Jumlah IP | Netmask |
| ----------- | ------------------------------------------------------------------------------------- | --------- | ------- |
| A1          | Hololive - Holo-EN                                                                    | 2         | /30     |
| A2          | Holo-EN - HoloAdvent                                                                  | 2         | /30     |
| A3          | Holo-EN - Holo-Myth                                                                   | 2         | /30     |
| A4          | Holo-Myth - Switch2 - Gura_Aine_Ina (309 Host) - Kiara_Calli (193 Host)               | 503       | /23     |
| A5          | HoloAdvent - Switch0 - FuwaMoco (5 Host) - Shiori_Nerissa (12 Host) - Biboo (10 Host) | 28        | /27     |
| A6          | Holo-Myth - HoloPromise - Router4 - Holo-Council                                      | 3         | /29     |
| A7          | Router4 - Tys (2 Host)                                                                | 3         | /29     |
| A8          | Holo-Council - Switch4 - Kronii_Mumei (39 Host) - Bae_Fauna (22 Host)                 | 62        | /26     |
| A9          | Hololive - Holo-JP                                                                    | 2         | /30     |
| A10         | Holo-JP - Switch1 - DEV_IS - GEN:0                                                    | 3         | /29     |
| A11         | DEV_IS - `Re:GLO$$` - Ririka_Raden (3 Host) - Ao (3 Host) - Hajime_Kanade (7 Host)    | 14        | /28     |
| A12         | GEN:0 - Switch3 - MiComet (1501 Host) - Sora_Robo_AZKi (542 Host) - GEN:1             | 2045      | /21     |
| A13         | GEN:1 - GAMERS                                                                        | 2         | /30     |
| A14         | GAMERS - Switch13 - Korone (51 Host) - Okayu (32 Host) - Mio (36 Host)                | 120       | /25     |
| A15         | GEN:1 - Member - FBK_Matsuri (321 Host) - Aki_Hachama (148 Host)                      | 470       | /23     |
| A16         | Hololive - Holp-ID                                                                    | 2         | /30     |
| A17         | Holo-ID - AREA15                                                                      | 2         | /30     |
| A18         | AREA15 - Switch6 - Risu (319 Host) - Moona (201 Host) - lofi (140 Host)               | 661       | /22     |
| A19         | Holo-ID - holoro                                                                      | 2         | /30     |
| A20         | Holo-ID - holoh3ro                                                                    | 2         | /30     |
| A21         | holoh3ro - Switch8 - Zeta (81 Host) - Kaela (71 Host) - Kobo (146 Host)               | 299       | /23     |
| A22         | holoro - Switch7 - Ollie (20 Host) - Anya (3 Host) - Reine (10 Host)                  | 34        | /26     |
| Total       |                                                                                       | 4263      | /19     |

# CPT VLSM

### Topologi

<img src="./img/pembag-subnet-cpt-topo.png" />

### Pembagian IP

Prefix IP: 10.67.xx.xx

| Subnet | Network ID   | Netmask               | Broadcast    | Range IP (Usable)           |
| ------ | ------------ | --------------------- | ------------ | --------------------------- |
| A12    | 10.67.2.0    | 255.255.248.0 (/21)   | 10.67.9.255  | 10.67.2.1 - 10.67.9.254     |
| A18    | 10.67.12.0   | 255.255.252.0 (/22)   | 10.67.15.255 | 10.67.12.1 - 10.67.15.254   |
| A15    | 10.67.10.128 | 255.255.254.0 (/23)   | 10.67.11.255 | 10.67.10.129 - 10.67.11.254 |
| A21    | 10.67.16.0   | 255.255.254.0 (/23)   | 10.67.17.255 | 10.67.16.1 - 10.67.17.254   |
| A4     | 10.67.1.76   | 255.255.254.0 (/23)   | 10.67.1.255  | 10.67.1.77 - 10.67.1.254    |
| A8     | 10.67.1.112  | 255.255.255.192 (/26) | 10.67.1.175  | 10.67.1.113 - 10.67.1.174   |
| A22    | 10.67.18.0   | 255.255.255.192 (/26) | 10.67.18.63  | 10.67.18.1 - 10.67.18.62    |
| A14    | 10.67.10.0   | 255.255.255.128 (/25) | 10.67.10.127 | 10.67.10.1 - 10.67.10.126   |
| A5     | 10.67.1.80   | 255.255.255.224 (/27) | 10.67.1.111  | 10.67.1.81 - 10.67.1.110    |
| A11    | 10.67.1.40   | 255.255.255.240 (/28) | 10.67.1.55   | 10.67.1.41 - 10.67.1.54     |
| A6     | 10.67.1.12   | 255.255.255.248 (/29) | 10.67.1.19   | 10.67.1.13 - 10.67.1.18     |
| A7     | 10.67.1.20   | 255.255.255.248 (/29) | 10.67.1.27   | 10.67.1.21 - 10.67.1.26     |
| A10    | 10.67.1.32   | 255.255.255.248 (/29) | 10.67.1.39   | 10.67.1.33 - 10.67.1.38     |
| A1     | 10.67.1.0    | 255.255.255.252 (/30) | 10.67.1.3    | 10.67.1.1 - 10.67.1.2       |
| A2     | 10.67.1.4    | 255.255.255.252 (/30) | 10.67.1.7    | 10.67.1.5 - 10.67.1.6       |
| A3     | 10.67.1.8    | 255.255.255.252 (/30) | 10.67.1.11   | 10.67.1.9 - 10.67.1.10      |
| A9     | 10.67.1.28   | 255.255.255.252 (/30) | 10.67.1.31   | 10.67.1.29 - 10.67.1.30     |
| A13    | 10.67.1.56   | 255.255.255.252 (/30) | 10.67.1.59   | 10.67.1.57 - 10.67.1.58     |
| A16    | 10.67.1.60   | 255.255.255.252 (/30) | 10.67.1.63   | 10.67.1.61 - 10.67.1.62     |
| A17    | 10.67.1.64   | 255.255.255.252 (/30) | 10.67.1.67   | 10.67.1.65 - 10.67.1.66     |
| A19    | 10.67.1.68   | 255.255.255.252 (/30) | 10.67.1.71   | 10.67.1.69 - 10.67.1.70     |
| A20    | 10.67.1.72   | 255.255.255.252 (/30) | 10.67.1.75   | 10.67.1.73 - 10.67.1.74     |

Total alokasi IP ini diurutkan berdasarkan jumlah host terbesar hingga terkecil.

### Tree

### Konfigurasi
