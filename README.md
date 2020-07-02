# Vastaukset 90/100 


## Tehtävä 1 
Hae kaikkien elokuvien nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Lumikki</td></tr><tr><td>Fantasia</td></tr><tr><td>Pinocchio</td></tr><tr><td>Dumbo</td></tr><tr><td>Bambi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat;
```

---



## Tehtävä 2 
Hae kaikkien elokuvien nimet ja julkaisuvuodet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Lumikki</td><td>1937</td></tr><tr><td>Fantasia</td><td>1940</td></tr><tr><td>Pinocchio</td><td>1940</td></tr><tr><td>Dumbo</td><td>1941</td></tr><tr><td>Bambi</td><td>1942</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi,vuosi FROM Elokuvat;
```
#### Mallivastaus
```sql
SELECT nimi, vuosi FROM Elokuvat;
```

---



## Tehtävä 3 
Hae kaikkien vuonna 1940 julkaistujen elokuvien nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Fantasia</td></tr><tr><td>Pinocchio</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat WHERE vuosi=1940;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat WHERE vuosi=1940;
```

---



## Tehtävä 4 
Hae ennen vuotta 1950 julkaistujen elokuvien nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Bambi</td><td>1942</td></tr><tr><td>4</td><td>Peter Pan</td><td>1953</td></tr><tr><td>5</td><td>Hiidenpata</td><td>1985</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Lumikki</td></tr><tr><td>Fantasia</td></tr><tr><td>Bambi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat WHERE vuosi<1950;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat WHERE vuosi<1950;
```

---



## Tehtävä 5 
Hae vuosina 1940–1950 julkaistujen elokuvien nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Bambi</td><td>1942</td></tr><tr><td>4</td><td>Peter Pan</td><td>1953</td></tr><tr><td>5</td><td>Hiidenpata</td><td>1985</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Fantasia</td></tr><tr><td>Bambi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat WHERE vuosi>=1940 AND vuosi<=1950;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat WHERE vuosi BETWEEN 1940 AND 1950;
```

---



## Tehtävä 6 
Hae ennen vuotta 1950 tai vuoden 1980 jälkeen julkaistujen elokuvien nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Bambi</td><td>1942</td></tr><tr><td>4</td><td>Peter Pan</td><td>1953</td></tr><tr><td>5</td><td>Hiidenpata</td><td>1985</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Lumikki</td></tr><tr><td>Fantasia</td></tr><tr><td>Bambi</td></tr><tr><td>Hiidenpata</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat WHERE vuosi < 1950 OR vuosi > 1980;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat WHERE vuosi<1950 OR vuosi>1980;
```

---



## Tehtävä 7 
Hae kaikkien elokuvien nimet, joita ei ole julkaistu vuonna 1940.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Lumikki</td></tr><tr><td>Dumbo</td></tr><tr><td>Bambi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat WHERE vuosi IS NOT 1940;
```
#### Mallivastaus
```sql
SELECT animal, species, size FROM Shrimps WHERE size<20 OR 200<size
```

---



## Tehtävä 8 
Hae kaikkien elokuvien nimet aakkosjärjestyksessä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Bambi</td></tr><tr><td>Dumbo</td></tr><tr><td>Fantasia</td></tr><tr><td>Lumikki</td></tr><tr><td>Pinocchio</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat ORDER BY nimi;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat ORDER BY nimi;
```

---



## Tehtävä 9 
Hae kaikkien elokuvien nimet käänteisessä aakkosjärjestyksessä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Pinocchio</td></tr><tr><td>Lumikki</td></tr><tr><td>Fantasia</td></tr><tr><td>Dumbo</td></tr><tr><td>Bambi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi FROM Elokuvat ORDER BY nimi DESC;
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat ORDER BY nimi DESC;
```

---



## Tehtävä 10 
Hae elokuvien nimet ja julkaisuvuodet ensisijaisesti käänteisessä järjestyksessä julkaisuvuoden mukaan, toissijaisesti aakkosjärjestyksessä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Bambi</td><td>1942</td></tr><tr><td>Dumbo</td><td>1941</td></tr><tr><td>Fantasia</td><td>1940</td></tr><tr><td>Pinocchio</td><td>1940</td></tr><tr><td>Lumikki</td><td>1937</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi,vuosi FROM Elokuvat ORDER BY vuosi DESC, nimi;
```
#### Mallivastaus
```sql
SELECT nimi, vuosi FROM Elokuvat ORDER BY vuosi DESC, nimi;
```

---



## Tehtävä 11 
Hae kaikki eri etunimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Nimet</i><table border=""><tbody><tr><th>id</th><th>etunimi</th><th>sukunimi</th></tr><tr><td>1</td><td>Anna</td><td>Korhonen</td></tr><tr><td>2</td><td>Anna</td><td>Virtanen</td></tr><tr><td>3</td><td>Pekka</td><td>Korhonen</td></tr><tr><td>4</td><td>Pekka</td><td>Lahtinen</td></tr><tr><td>5</td><td>Pekka</td><td>Virtanen</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Anna</td></tr><tr><td>Pekka</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT DISTINCT etunimi FROM Nimet;
```
#### Mallivastaus
```sql
SELECT DISTINCT etunimi FROM Nimet;
```

---



## Tehtävä 12 
Hae kaikki eri nimet.

**Taulut**

<table><tbody><tr valign="top"><td><i>Nimet</i><table border=""><tbody><tr><th>id</th><th>etunimi</th><th>sukunimi</th></tr><tr><td>1</td><td>Anna</td><td>Korhonen</td></tr><tr><td>2</td><td>Anna</td><td>Korhonen</td></tr><tr><td>3</td><td>Pekka</td><td>Korhonen</td></tr><tr><td>4</td><td>Pekka</td><td>Virtanen</td></tr><tr><td>5</td><td>Pekka</td><td>Virtanen</td></tr><tr><td>6</td><td>Pekka</td><td>Virtanen</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Anna</td><td>Korhonen</td></tr><tr><td>Pekka</td><td>Korhonen</td></tr><tr><td>Pekka</td><td>Virtanen</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT DISTINCT etunimi, sukunimi FROM Nimet;
```
#### Mallivastaus
```sql
SELECT DISTINCT etunimi, sukunimi FROM Nimet;
```

---



## Tehtävä 13 
Hae työntekijöiden määrä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th></tr><tr><td>1</td><td>Uolevi</td><td>2500</td></tr><tr><td>2</td><td>Maija</td><td>3000</td></tr><tr><td>3</td><td>Liisa</td><td>5000</td></tr><tr><td>4</td><td>Kaaleppi</td><td>1500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT COUNT(*) FROM Tyontekijat;
```
#### Mallivastaus
```sql
SELECT COUNT(*) FROM Tyontekijat;
```

---



## Tehtävä 14 
Hae niiden työntekijöiden määrä, joiden palkka on yli 2000.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th></tr><tr><td>1</td><td>Uolevi</td><td>2500</td></tr><tr><td>2</td><td>Maija</td><td>3000</td></tr><tr><td>3</td><td>Liisa</td><td>5000</td></tr><tr><td>4</td><td>Kaaleppi</td><td>1500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>3</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT COUNT(*) FROM Tyontekijat WHERE palkka > 2000;
```
#### Mallivastaus
```sql
SELECT COUNT(*) FROM Tyontekijat WHERE palkka>2000;
```

---



## Tehtävä 15 
Hae työntekijöiden yhteispalkka.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th></tr><tr><td>1</td><td>Uolevi</td><td>2500</td></tr><tr><td>2</td><td>Maija</td><td>3000</td></tr><tr><td>3</td><td>Liisa</td><td>5000</td></tr><tr><td>4</td><td>Kaaleppi</td><td>1500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>12000</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT SUM(palkka) FROM Tyontekijat;
```
#### Mallivastaus
```sql
SELECT SUM(palkka) FROM Tyontekijat;
```

---



## Tehtävä 16 
Hae suurin työntekijän palkka.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th></tr><tr><td>1</td><td>Uolevi</td><td>2500</td></tr><tr><td>2</td><td>Maija</td><td>3000</td></tr><tr><td>3</td><td>Liisa</td><td>5000</td></tr><tr><td>4</td><td>Kaaleppi</td><td>1500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>5000</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT MAX(palkka) FROM Tyontekijat;
```
#### Mallivastaus
```sql
SELECT MAX(palkka) FROM Tyontekijat;
```

---



## Tehtävä 17 
Hae eri yritysten määrä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th><th>yritys</th></tr><tr><td>1</td><td>Uolevi</td><td>5000</td><td>Google</td></tr><tr><td>2</td><td>Maija</td><td>6000</td><td>Google</td></tr><tr><td>3</td><td>Liisa</td><td>2000</td><td>Amazon</td></tr><tr><td>4</td><td>Kaaleppi</td><td>7500</td><td>Microsoft</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>3</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT COUNT(DISTINCT yritys) FROM Tyontekijat;
```
#### Mallivastaus
```sql
SELECT COUNT(DISTINCT yritys) FROM Tyontekijat;
```

---



## Tehtävä 18 
Hae jokaisen yrityksen työntekijöiden määrä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th><th>yritys</th></tr><tr><td>1</td><td>Uolevi</td><td>5000</td><td>Google</td></tr><tr><td>2</td><td>Maija</td><td>6000</td><td>Google</td></tr><tr><td>3</td><td>Liisa</td><td>2000</td><td>Amazon</td></tr><tr><td>4</td><td>Kaaleppi</td><td>7500</td><td>Microsoft</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Google</td><td>2</td></tr><tr><td>Amazon</td><td>1</td></tr><tr><td>Microsoft</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT yritys, COUNT(*) FROM Tyontekijat GROUP BY yritys;
```
#### Mallivastaus
```sql
SELECT yritys, COUNT(*) FROM Tyontekijat GROUP BY yritys;
```

---



## Tehtävä 19 
Hae jokaisesta yrityksestä suurin työntekijän palkka.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th><th>yritys</th></tr><tr><td>1</td><td>Uolevi</td><td>5000</td><td>Google</td></tr><tr><td>2</td><td>Maija</td><td>6000</td><td>Google</td></tr><tr><td>3</td><td>Liisa</td><td>2000</td><td>Amazon</td></tr><tr><td>4</td><td>Kaaleppi</td><td>7500</td><td>Microsoft</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Google</td><td>6000</td></tr><tr><td>Amazon</td><td>2000</td></tr><tr><td>Microsoft</td><td>7500</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT yritys, MAX(palkka) FROM Tyontekijat GROUP BY yritys;
```
#### Mallivastaus
```sql
SELECT yritys, MAX(palkka) FROM Tyontekijat GROUP BY yritys;
```

---



## Tehtävä 20 
Näytä suurin työntekijän palkka yrityksistä, joissa se on ainakin 5000.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tyontekijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>palkka</th><th>yritys</th></tr><tr><td>1</td><td>Uolevi</td><td>5000</td><td>Google</td></tr><tr><td>2</td><td>Maija</td><td>6000</td><td>Google</td></tr><tr><td>3</td><td>Liisa</td><td>2000</td><td>Amazon</td></tr><tr><td>4</td><td>Kaaleppi</td><td>7500</td><td>Microsoft</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Google</td><td>6000</td></tr><tr><td>Microsoft</td><td>7500</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT yritys, MAX(palkka) FROM Tyontekijat WHERE palkka >= 5000 GROUP BY yritys;
```
#### Mallivastaus
```sql
SELECT yritys, MAX(palkka) FROM Tyontekijat GROUP BY yritys HAVING MAX(palkka)>=5000;
```

---



## Tehtävä 21 
Muodosta tuloslista, jossa näkyvät kaikki tulokset.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>250</td></tr><tr><td>Uolevi</td><td>300</td></tr><tr><td>Maija</td><td>100</td></tr><tr><td>Maija</td><td>350</td></tr><tr><td>Kaaleppi</td><td>500</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, Tulokset.tulos FROM Pelaajat, Tulokset WHERE Tulokset.pelaaja_id = Pelaajat.id;
```
#### Mallivastaus
```sql
SELECT P.nimi, T.tulos FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id;
```

---



## Tehtävä 22 
Muodosta tuloslista, jossa näkyvät Uolevin tulokset.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>250</td></tr><tr><td>Uolevi</td><td>300</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, Tulokset.tulos FROM Pelaajat, Tulokset WHERE Tulokset.pelaaja_id = Pelaajat.id AND Pelaajat.nimi='Uolevi';
```
#### Mallivastaus
```sql
SELECT P.nimi, T.tulos FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id AND P.nimi='Uolevi';
```

---



## Tehtävä 23 
Muodosta tuloslista, jossa näkyvät tulokset, jotka ovat parempia kuin 250.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>400</td></tr><tr><td>6</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>300</td></tr><tr><td>Maija</td><td>350</td></tr><tr><td>Kaaleppi</td><td>400</td></tr><tr><td>Kaaleppi</td><td>500</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, Tulokset.tulos FROM Pelaajat, Tulokset WHERE Tulokset.pelaaja_id = Pelaajat.id AND Tulokset.tulos > 250;
```
#### Mallivastaus
```sql
SELECT P.nimi, T.tulos FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id AND T.tulos>250;
```

---



## Tehtävä 24 
Muodosta tuloslista, jossa näkyy kaikki tulokset järjestettynä ensisijaisesti käänteisesti pistemäärän mukaan ja toissijaisesti nimen mukaan.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>350</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Kaaleppi</td><td>500</td></tr><tr><td>Maija</td><td>350</td></tr><tr><td>Uolevi</td><td>350</td></tr><tr><td>Uolevi</td><td>250</td></tr><tr><td>Maija</td><td>100</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, Tulokset.tulos FROM Pelaajat, Tulokset WHERE Tulokset.pelaaja_id = Pelaajat.id ORDER BY Tulokset.tulos DESC, Pelaajat.nimi;
```
#### Mallivastaus
```sql
SELECT P.nimi, T.tulos FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id ORDER BY T.tulos DESC, P.nimi;
```

---



## Tehtävä 25 
Ilmoita jokaisesta pelaajasta, mikä on hänen paras tuloksensa. Voit olettaa, että jokaisella pelaajalla on ainakin yksi tulos.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>300</td></tr><tr><td>Maija</td><td>350</td></tr><tr><td>Kaaleppi</td><td>500</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, MAX(Tulokset.tulos) FROM Pelaajat, Tulokset WHERE Tulokset.pelaaja_id = Pelaajat.id GROUP BY nimi;
```
#### Mallivastaus
```sql
SELECT P.nimi, MAX(T.tulos) FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id GROUP BY P.id;
```

---



## Tehtävä 26 
Ilmoita jokaisesta pelaajasta, montako tulosta hänellä on. Voit olettaa, että jokaisella pelaajalla on ainakin yksi tulos.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>2</td></tr><tr><td>Kaaleppi</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi, COUNT(*) FROM Pelaajat, Tulokset WHERE pelaaja_id = Pelaajat.id GROUP BY nimi;
```
#### Mallivastaus
```sql
SELECT P.nimi, COUNT(T.tulos) FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id GROUP BY P.id;
```

---



## Tehtävä 27 
Hae kaikista suorituksista opiskelijan nimi, kurssin nimi ja arvosana.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>Ohpe</td><td>3</td></tr><tr><td>Uolevi</td><td>Ohja</td><td>4</td></tr><tr><td>Maija</td><td>Ohpe</td><td>2</td></tr><tr><td>Maija</td><td>Lama</td><td>5</td></tr><tr><td>Kaaleppi</td><td>Tira</td><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, Kurssit.nimi, arvosana FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.kurssi_id = Kurssit.id AND Suoritukset.opiskelija_id = Opiskelijat.id;
```
#### Mallivastaus
```sql
SELECT O.nimi, K.nimi, S.arvosana FROM Opiskelijat O, Kurssit K, Suoritukset S WHERE O.id=S.opiskelija_id AND K.id=S.kurssi_id;
```

---



## Tehtävä 28 
Hae kaikista Uolevin suorituksista kurssin nimi ja arvosana.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Ohpe</td><td>3</td></tr><tr><td>Ohja</td><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kurssit.nimi, arvosana FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.kurssi_id = Kurssit.id AND Suoritukset.opiskelija_id = Opiskelijat.id AND Opiskelijat.nimi = 'Uolevi';
```
#### Mallivastaus
```sql
SELECT K.nimi, S.arvosana FROM Opiskelijat O, Kurssit K, Suoritukset S WHERE O.id=S.opiskelija_id AND K.id=S.kurssi_id AND O.nimi='Uolevi';
```

---



## Tehtävä 29 
Hae kaikista Ohpen suorituksista opiskelijan nimi ja arvosana.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>3</td></tr><tr><td>Maija</td><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, arvosana FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.kurssi_id = Kurssit.id AND Suoritukset.opiskelija_id = Opiskelijat.id AND Kurssit.nimi = 'Ohpe';
```
#### Mallivastaus
```sql
SELECT O.nimi, S.arvosana FROM Opiskelijat O, Kurssit K, Suoritukset S WHERE O.id=S.opiskelija_id AND K.id=S.kurssi_id AND K.nimi='Ohpe';
```

---



## Tehtävä 30 
Hae kaikki suoritukset, joissa arvosana on 4 tai 5.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>Ohja</td><td>4</td></tr><tr><td>Maija</td><td>Lama</td><td>5</td></tr><tr><td>Kaaleppi</td><td>Tira</td><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, Kurssit.nimi, arvosana FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.kurssi_id = Kurssit.id AND Suoritukset.opiskelija_id = Opiskelijat.id AND (Suoritukset.arvosana = 4 OR Suoritukset.arvosana = 5);;
```
#### Mallivastaus
```sql
SELECT O.nimi, K.nimi, S.arvosana FROM Opiskelijat O, Kurssit K, Suoritukset S WHERE O.id=S.opiskelija_id AND K.id=S.kurssi_id AND S.arvosana BETWEEN 4 AND 5;
```

---



## Tehtävä 31 
Hae jokaisesta opiskelijasta suoritusten määrä. Voit olettaa, että jokaisella opiskelijalla on ainakin yksi suoritus.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>2</td></tr><tr><td>Kaaleppi</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, COUNT(*) FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.opiskelija_id = Opiskelijat.id AND Suoritukset.kurssi_id = Kurssit.id GROUP BY Opiskelijat.nimi;
```
#### Mallivastaus
```sql
SELECT O.nimi, COUNT(*) FROM Opiskelijat O, Suoritukset S WHERE O.id=S.opiskelija_id GROUP BY O.id;
```

---



## Tehtävä 32 
Hae jokaisesta opiskelijasta paras suorituksen arvosana. Voit olettaa, että jokaisella opiskelijalla on ainakin yksi suoritus.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>4</td><td>5</td></tr><tr><td>3</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>4</td></tr><tr><td>Maija</td><td>5</td></tr><tr><td>Kaaleppi</td><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, MAX(Suoritukset.arvosana) FROM Opiskelijat, Kurssit, Suoritukset WHERE Suoritukset.opiskelija_id = Opiskelijat.id AND Suoritukset.kurssi_id = Kurssit.id GROUP BY Opiskelijat.nimi;
```
#### Mallivastaus
```sql
SELECT O.nimi, MAX(S.arvosana) FROM Opiskelijat O, Suoritukset S WHERE O.id=S.opiskelija_id GROUP BY O.id;
```

---



## Tehtävä 33 
Hae tiedot kaikista lentoyhteyksistä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kaupungit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Helsinki</td></tr><tr><td>2</td><td>Tukholma</td></tr><tr><td>3</td><td>Oslo</td></tr><tr><td>4</td><td>Turku</td></tr></tbody></table></td><td width="20"></td><td><i>Lennot</i><table border=""><tbody><tr><th>id</th><th>mista_id</th><th>minne_id</th></tr><tr><td>1</td><td>1</td><td>2</td></tr><tr><td>2</td><td>1</td><td>3</td></tr><tr><td>3</td><td>2</td><td>3</td></tr><tr><td>4</td><td>2</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Helsinki</td><td>Tukholma</td></tr><tr><td>Helsinki</td><td>Oslo</td></tr><tr><td>Tukholma</td><td>Oslo</td></tr><tr><td>Tukholma</td><td>Turku</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT mista.nimi, minne.nimi FROM Kaupungit mista, Kaupungit minne, Lennot WHERE Lennot.mista_id = mista.id AND Lennot.minne_id = minne.id;
```
#### Mallivastaus
```sql
SELECT A.nimi, B.nimi FROM Kaupungit A, Kaupungit B, Lennot L WHERE L.mista_id=A.id AND L.minne_id=B.id;
```

---



## Tehtävä 34 
Hae kohteet kaikista lennoista, jotka lähtevät Helsingistä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kaupungit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Helsinki</td></tr><tr><td>2</td><td>Tukholma</td></tr><tr><td>3</td><td>Oslo</td></tr><tr><td>4</td><td>Turku</td></tr></tbody></table></td><td width="20"></td><td><i>Lennot</i><table border=""><tbody><tr><th>id</th><th>mista_id</th><th>minne_id</th></tr><tr><td>1</td><td>1</td><td>2</td></tr><tr><td>2</td><td>1</td><td>3</td></tr><tr><td>3</td><td>2</td><td>3</td></tr><tr><td>4</td><td>2</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Tukholma</td></tr><tr><td>Oslo</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT k2.nimi AS minne
FROM Lennot, Kaupungit AS k1, Kaupungit AS k2
WHERE Lennot.mista_id = k1.id
AND Lennot.minne_id = k2.id AND k1.nimi = 'Helsinki'
ORDER BY Lennot.mista_id;
```
#### Mallivastaus
```sql
SELECT B.nimi FROM Kaupungit A, Kaupungit B, Lennot L WHERE L.mista_id=A.id AND L.minne_id=B.id AND A.nimi='Helsinki';
```

---



## Tehtävä 35 
Ilmoita jokaisesta pelaajasta, montako tulosta hänellä on (myös vaikka ei olisi tuloksia).

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>250</td></tr><tr><td>2</td><td>1</td><td>300</td></tr><tr><td>3</td><td>2</td><td>100</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>2</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>3</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Pelaajat.nimi, (SELECT COUNT(*) FROM Tulokset
WHERE Pelaajat.id = Tulokset.pelaaja_id)
FROM Pelaajat;
```
#### Mallivastaus
```sql
SELECT P.nimi, COUNT(T.tulos) FROM Pelaajat P LEFT JOIN Tulokset T ON P.id=T.pelaaja_id GROUP BY P.id;
```

---



## Tehtävä 36 
Hae jokaisesta opiskelijasta suoritusten määrä (myös vaikka ei olisi suorituksia).

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>3</td><td>4</td></tr><tr><td>2</td><td>4</td><td>5</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>3</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, (SELECT COUNT(*) FROM Suoritukset
WHERE Opiskelijat.id = Suoritukset.opiskelija_id)
FROM Opiskelijat;
```
#### Mallivastaus
```sql
SELECT O.nimi, COUNT(S.arvosana) FROM Opiskelijat O LEFT JOIN Suoritukset S ON O.id=S.opiskelija_id GROUP BY O.id;
```

---



## Tehtävä 37 
Hae jokaisesta kurssista suorittajien määrä (myös vaikka ei olisi suorituksia).

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>2</td><td>5</td></tr><tr><td>3</td><td>4</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Ohpe</td><td>2</td></tr><tr><td>Ohja</td><td>2</td></tr><tr><td>Tira</td><td>0</td></tr><tr><td>Lama</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kurssit.nimi, (SELECT COUNT(*) FROM Suoritukset
WHERE Kurssit.id = Suoritukset.kurssi_id)
FROM Kurssit;
```
#### Mallivastaus
```sql
SELECT K.nimi, COUNT(S.arvosana) FROM Kurssit K LEFT JOIN Suoritukset S ON K.id=S.kurssi_id GROUP BY K.id;
```

---



## Tehtävä 38 
Hae nimet kaikista kursseista, joita on suoritettu ainakin kerran.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>2</td><td>5</td></tr><tr><td>3</td><td>4</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Ohpe</td></tr><tr><td>Ohja</td></tr><tr><td>Lama</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT DISTINCT Kurssit.nimi
FROM Opiskelijat, Kurssit, Suoritukset
WHERE Opiskelijat.id = Suoritukset.opiskelija_id
AND Kurssit.id = Suoritukset.kurssi_id
ORDER BY Suoritukset.arvosana;
```
#### Mallivastaus
```sql
SELECT DISTINCT K.nimi FROM Kurssit K, Suoritukset S WHERE K.id=S.kurssi_id;
```

---



## Tehtävä 39 
Hae nimet kaikista kursseista, joita ei ole suoritettu kertaakaan.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Kurssit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Ohpe</td></tr><tr><td>2</td><td>Ohja</td></tr><tr><td>3</td><td>Tira</td></tr><tr><td>4</td><td>Lama</td></tr></tbody></table></td><td width="20"></td><td><i>Suoritukset</i><table border=""><tbody><tr><th>opiskelija_id</th><th>kurssi_id</th><th>arvosana</th></tr><tr><td>1</td><td>1</td><td>3</td></tr><tr><td>1</td><td>2</td><td>4</td></tr><tr><td>2</td><td>1</td><td>2</td></tr><tr><td>2</td><td>2</td><td>5</td></tr><tr><td>3</td><td>4</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Tira</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kurssit.nimi FROM Kurssit
LEFT JOIN Suoritukset ON Kurssit.id = Suoritukset.kurssi_id
WHERE Suoritukset.kurssi_id IS NULL;
```
#### Mallivastaus
```sql
SELECT K.nimi FROM Kurssit K LEFT JOIN Suoritukset S ON K.id=S.kurssi_id GROUP BY K.id HAVING COUNT(S.arvosana)=0;
```

---



## Tehtävä 40 
Hae jokaisesta kaupungista, montako lentoa sieltä lähtee (myös vaikka ei olisi lentoja).

**Taulut**

<table><tbody><tr valign="top"><td><i>Kaupungit</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Helsinki</td></tr><tr><td>2</td><td>Tukholma</td></tr><tr><td>3</td><td>Oslo</td></tr><tr><td>4</td><td>Turku</td></tr></tbody></table></td><td width="20"></td><td><i>Lennot</i><table border=""><tbody><tr><th>id</th><th>mista_id</th><th>minne_id</th></tr><tr><td>1</td><td>1</td><td>2</td></tr><tr><td>2</td><td>1</td><td>3</td></tr><tr><td>3</td><td>2</td><td>3</td></tr><tr><td>4</td><td>3</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Helsinki</td><td>2</td></tr><tr><td>Tukholma</td><td>1</td></tr><tr><td>Oslo</td><td>1</td></tr><tr><td>Turku</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kaupungit.nimi, (SELECT COUNT(*) FROM Lennot
WHERE Kaupungit.id = Lennot.mista_id)
FROM Kaupungit;
```
#### Mallivastaus
```sql
SELECT K.nimi, COUNT(L.minne_id) FROM Kaupungit K LEFT JOIN Lennot L ON K.id=L.mista_id GROUP BY K.id;
```

---



## Tehtävä 41 
Hae jokaisen tuotteen hinta kaksinkertaisena.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>5</td></tr><tr><td>2</td><td>lanttu</td><td>8</td></tr><tr><td>3</td><td>nauris</td><td>6</td></tr><tr><td>4</td><td>porkkana</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>selleri</td><td>10</td></tr><tr><td>lanttu</td><td>16</td></tr><tr><td>nauris</td><td>12</td></tr><tr><td>porkkana</td><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi, (Tuotteet.hinta * 2) FROM Tuotteet;
```
#### Mallivastaus
```sql
SELECT nimi, hinta*2 FROM Tuotteet;
```

---



## Tehtävä 42 
Hae kaikki tuotteet, joiden hinta on parillinen.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>5</td></tr><tr><td>2</td><td>lanttu</td><td>8</td></tr><tr><td>3</td><td>nauris</td><td>7</td></tr><tr><td>4</td><td>porkkana</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td><td>8</td></tr><tr><td>porkkana</td><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi, Tuotteet.hinta
FROM Tuotteet WHERE (Tuotteet.hinta % 2 == 0);
```
#### Mallivastaus
```sql
SELECT nimi, hinta FROM Tuotteet WHERE hinta%2=0;
```

---



## Tehtävä 43 
Hae jokaisen sanan pituus merkkeinä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td><td>5</td></tr><tr><td>banaani</td><td>7</td></tr><tr><td>cembalo</td><td>7</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana, LENGTH(sana) FROM Sanat;
```
#### Mallivastaus
```sql
SELECT sana, LENGTH(sana) FROM Sanat;
```

---



## Tehtävä 44 
Hae kaikki sanat, joiden pituus on alle 6 merkkiä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Sanat.sana FROM Sanat WHERE LENGTH(sana) <  6;
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat WHERE LENGTH(sana)<6;
```

---



## Tehtävä 45 
Hae sanat järjestettynä ensisijaisesti pituuden mukaan ja toissijaisesti aakkosjärjestyksen mukaan.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>banaani</td></tr><tr><td>2</td><td>aakkonen</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>banaani</td></tr><tr><td>cembalo</td></tr><tr><td>aakkonen</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Sanat.sana FROM Sanat ORDER BY LENGTH(Sanat.sana), Sanat.sana;
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat ORDER BY LENGTH(sana), sana;
```

---



## Tehtävä 46 
Hae käyttäjien koko nimet yhtenä sarakkeena.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>etunimi</th><th>sukunimi</th></tr><tr><td>1</td><td>Liisa</td><td>Virtanen</td></tr><tr><td>2</td><td>Anna</td><td>Korhonen</td></tr><tr><td>3</td><td>Kalle</td><td>Ojala</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Liisa Virtanen</td></tr><tr><td>Anna Korhonen</td></tr><tr><td>Kalle Ojala</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT etunimi || ' ' || sukunimi FROM Kayttajat;
```
#### Mallivastaus
```sql
SELECT etunimi || ' ' || sukunimi FROM Kayttajat;
```

---



## Tehtävä 47 
Hae kaikkien sanojen yhteispituus.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>19</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT SUM(LENGTH(sana)) FROM Sanat;
```
#### Mallivastaus
```sql
SELECT SUM(LENGTH(sana)) FROM Sanat;
```

---



## Tehtävä 48 
Laske jokaisen tilauksen yhteishinta.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tilaukset</i><table border=""><tbody><tr><th>id</th><th>tuote</th><th>hinta</th><th>maara</th></tr><tr><td>1</td><td>lanttu</td><td>4</td><td>10</td></tr><tr><td>2</td><td>selleri</td><td>7</td><td>20</td></tr><tr><td>3</td><td>nauris</td><td>5</td><td>15</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td><td>40</td></tr><tr><td>selleri</td><td>140</td></tr><tr><td>nauris</td><td>75</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tilaukset.tuote,
       (Tilaukset.hinta * Tilaukset.maara)
  FROM Tilaukset;
```
#### Mallivastaus
```sql
SELECT tuote, hinta*maara FROM Tilaukset;
```

---



## Tehtävä 49 
Laske kaikkien tilausten yhteishintojen summa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tilaukset</i><table border=""><tbody><tr><th>id</th><th>tuote</th><th>hinta</th><th>maara</th></tr><tr><td>1</td><td>lanttu</td><td>4</td><td>10</td></tr><tr><td>2</td><td>selleri</td><td>7</td><td>20</td></tr><tr><td>3</td><td>nauris</td><td>5</td><td>15</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>255</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT SUM(hinta *maara) FROM Tilaukset;
```
#### Mallivastaus
```sql
SELECT SUM(hinta*maara) FROM Tilaukset;
```

---



## Tehtävä 50 
Hae kaikkien elokuvien nimet, jotka on julkaistu karkausvuonna. (Vuosi on karkausvuosi, jos se on jaollinen 4:llä. Jos vuosi on jaollinen 100:lla, se on karkausvuosi vain, jos se on myös jaollinen 400:lla.)

**Taulut**

<table><tbody><tr valign="top"><td><i>Elokuvat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vuosi</th></tr><tr><td>1</td><td>Lumikki</td><td>1937</td></tr><tr><td>2</td><td>Fantasia</td><td>1940</td></tr><tr><td>3</td><td>Pinocchio</td><td>1940</td></tr><tr><td>4</td><td>Dumbo</td><td>1941</td></tr><tr><td>5</td><td>Bambi</td><td>1942</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Fantasia</td></tr><tr><td>Pinocchio</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Elokuvat.nimi FROM Elokuvat WHERE (Elokuvat.vuosi % 4 == 0 AND Elokuvat.vuosi % 100
IS NOT 0 OR Elokuvat.vuosi % 400 == 0);
```
#### Mallivastaus
```sql
SELECT nimi FROM Elokuvat WHERE vuosi%4=0 AND (vuosi%100<>0 OR vuosi%400=0);
```

---



## Tehtävä 51 
Hae kaikki tuotteet, joiden hinta on halvin hinta.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>5</td></tr><tr><td>3</td><td>retiisi</td><td>8</td></tr><tr><td>4</td><td>nauris</td><td>5</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td></tr><tr><td>nauris</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi FROM Tuotteet
WHERE Tuotteet.hinta IN (SELECT MIN(Tuotteet.hinta) FROM Tuotteet);
```
#### Mallivastaus
```sql
SELECT nimi FROM Tuotteet WHERE hinta=(SELECT MIN(hinta) FROM Tuotteet);
```

---



## Tehtävä 52 
Hae kaikki tuotteet, joiden hinta on enintään kaksinkertainen halvimpaan hintaan verrattuna.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>5</td></tr><tr><td>4</td><td>nauris</td><td>6</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td></tr><tr><td>retiisi</td></tr><tr><td>nauris</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi FROM Tuotteet
WHERE Tuotteet.hinta <=
((SELECT MIN(Tuotteet.hinta) FROM Tuotteet) * 2);
```
#### Mallivastaus
```sql
SELECT nimi FROM Tuotteet WHERE hinta <= 2*(SELECT MIN(hinta) FROM Tuotteet);
```

---



## Tehtävä 53 
Hae kaikki tuotteet, joiden hintaa ei ole millään muulla tuotteella.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>5</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>5</td></tr><tr><td>4</td><td>nauris</td><td>6</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td></tr><tr><td>nauris</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT t1.nimi
FROM Tuotteet t1
WHERE t1.hinta
NOT IN (SELECT t2.hinta
    FROM Tuotteet t2
    WHERE t2.id <> t1.id);
```
#### Mallivastaus
```sql
SELECT nimi FROM Tuotteet WHERE hinta IN (SELECT hinta FROM Tuotteet GROUP BY hinta HAVING COUNT(*)=1);
```

---



## Tehtävä 54 
Hae aakkosjärjestyksessä ensimmäinen sana.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat ORDER BY sana LIMIT 1;
```
#### Mallivastaus
```sql
SELECT MIN(sana) FROM Sanat;
```

---



## Tehtävä 55 
Hae aakkosjärjestyksessä toinen sana. Voit olettaa, että taulussa ei ole kahta samaa sanaa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>banaani</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat ORDER BY sana LIMIT 1 OFFSET 1;
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat ORDER BY sana LIMIT 1 OFFSET 1;
```

---



## Tehtävä 56 
Hae kaikki sanat paitsi aakkosjärjestyksessä ensimmäinen. Voit olettaa, että taulussa ei ole kahta samaa sanaa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>banaani</td></tr><tr><td>cembalo</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat ORDER BY sana LIMIT 10 OFFSET 1;
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat ORDER BY sana LIMIT (SELECT COUNT(*)-1 FROM Sanat) OFFSET 1;
```

---



## Tehtävä 57 
Hae kaikki sanat, joissa esiintyy i-kirjain.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr><tr><td>banaani</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat WHERE sana LIKE '%i%';
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat WHERE sana LIKE '%i%';
```

---



## Tehtävä 58 
Hae kaikki sanat, jotka alkavat a-kirjaimella.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat WHERE sana LIKE 'a%';
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat WHERE sana LIKE 'a%';
```

---



## Tehtävä 59 
Hae kaikki sanat, joissa on tasan viisi kirjainta ja toinen kirjain on p.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Sanat.sana
FROM Sanat
WHERE LENGTH(Sanat.sana) = 5
AND Sanat.sana LIKE '%p%%%';
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat WHERE sana LIKE '_p___';
```

---



## Tehtävä 60 
Hae kaikki sanat, joissa on tasan kaksi a-kirjainta.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>apina</td></tr><tr><td>2</td><td>banaani</td></tr><tr><td>3</td><td>cembalo</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Sanat.sana FROM Sanat WHERE (LENGTH(Sanat.sana) - LENGTH(REPLACE(Sanat.sana, 'a', '')) = 2);
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat WHERE sana LIKE '%a%a%' AND sana NOT LIKE '%a%a%a%';
```

---



## Tehtävä 61 
Hae jokaisesta käyttäjästä tieto, monessako ryhmässä hän on.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>tunnus</th></tr><tr><td>1</td><td>uolevi</td></tr><tr><td>2</td><td>maija</td></tr><tr><td>3</td><td>kaaleppi</td></tr><tr><td>4</td><td>liisa</td></tr></tbody></table></td><td width="20"></td><td><i>Ryhmat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>puput</td></tr><tr><td>2</td><td>kilit</td></tr></tbody></table></td><td width="20"></td><td><i>Oikeudet</i><table border=""><tbody><tr><th>kayttaja_id</th><th>ryhma_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>2</td><td>1</td></tr><tr><td>3</td><td>1</td></tr><tr><td>3</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>uolevi</td><td>1</td></tr><tr><td>maija</td><td>1</td></tr><tr><td>kaaleppi</td><td>2</td></tr><tr><td>liisa</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kayttajat.tunnus, (SELECT COUNT(*) 
    FROM Oikeudet, Ryhmat
    WHERE Kayttajat.id = Oikeudet.kayttaja_id
    AND Oikeudet.ryhma_id = Ryhmat.id)
    FROM Kayttajat
```
#### Mallivastaus
```sql
SELECT K.tunnus, COUNT(O.ryhma_id) FROM Kayttajat K LEFT JOIN Oikeudet O ON K.id=O.kayttaja_id GROUP BY K.id;
```

---



## Tehtävä 62 
Hae jokaisesta ryhmästä tieto, montako käyttäjää siihen kuuluu.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>tunnus</th></tr><tr><td>1</td><td>uolevi</td></tr><tr><td>2</td><td>maija</td></tr><tr><td>3</td><td>kaaleppi</td></tr><tr><td>4</td><td>liisa</td></tr></tbody></table></td><td width="20"></td><td><i>Ryhmat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>puput</td></tr><tr><td>2</td><td>kilit</td></tr></tbody></table></td><td width="20"></td><td><i>Oikeudet</i><table border=""><tbody><tr><th>kayttaja_id</th><th>ryhma_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>2</td><td>1</td></tr><tr><td>3</td><td>1</td></tr><tr><td>3</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>puput</td><td>3</td></tr><tr><td>kilit</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Ryhmat.nimi, (SELECT COUNT(Oikeudet.ryhma_id)
FROM Oikeudet WHERE Oikeudet.ryhma_id = Ryhmat.id) FROM Ryhmat;
```
#### Mallivastaus
```sql
SELECT R.nimi, COUNT(O.kayttaja_id) FROM Ryhmat R LEFT JOIN Oikeudet O ON R.id=O.ryhma_id GROUP BY R.id;
```

---



## Tehtävä 63 
Hae kaikki käyttäjät, jotka kuuluvat yli yhteen ryhmään.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>tunnus</th></tr><tr><td>1</td><td>uolevi</td></tr><tr><td>2</td><td>maija</td></tr><tr><td>3</td><td>kaaleppi</td></tr><tr><td>4</td><td>liisa</td></tr></tbody></table></td><td width="20"></td><td><i>Ryhmat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>puput</td></tr><tr><td>2</td><td>kilit</td></tr></tbody></table></td><td width="20"></td><td><i>Oikeudet</i><table border=""><tbody><tr><th>kayttaja_id</th><th>ryhma_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>2</td><td>1</td></tr><tr><td>3</td><td>1</td></tr><tr><td>3</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>kaaleppi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kayttajat.tunnus
FROM Kayttajat
WHERE ((SELECT COUNT(Oikeudet.kayttaja_id)
FROM Oikeudet WHERE Oikeudet.kayttaja_id = Kayttajat.id) >= 2);
```
#### Mallivastaus
```sql
SELECT K.tunnus FROM Kayttajat K LEFT JOIN Oikeudet O ON K.id=O.kayttaja_id GROUP BY K.id HAVING COUNT(O.ryhma_id) > 1;
```

---



## Tehtävä 64 
Hae kaikki käyttäjät, jotka kuuluvat ainakin yhteen samaan ryhmään käyttäjän "uolevi" kanssa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>tunnus</th></tr><tr><td>1</td><td>uolevi</td></tr><tr><td>2</td><td>maija</td></tr><tr><td>3</td><td>kaaleppi</td></tr><tr><td>4</td><td>liisa</td></tr></tbody></table></td><td width="20"></td><td><i>Ryhmat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>puput</td></tr><tr><td>2</td><td>kilit</td></tr></tbody></table></td><td width="20"></td><td><i>Oikeudet</i><table border=""><tbody><tr><th>kayttaja_id</th><th>ryhma_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>1</td><td>2</td></tr><tr><td>2</td><td>1</td></tr><tr><td>4</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>uolevi</td></tr><tr><td>maija</td></tr><tr><td>liisa</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kayttajat.tunnus
FROM Kayttajat WHERE Kayttajat.id
IN (SELECT Oikeudet.kayttaja_id FROM Oikeudet WHERE Oikeudet.ryhma_id
 IN (SELECT Oikeudet.ryhma_id FROM Oikeudet WHERE Oikeudet.kayttaja_id = 1));
```
#### Mallivastaus
```sql
SELECT DISTINCT A.tunnus FROM Kayttajat A, Kayttajat B, Oikeudet X, Oikeudet Y WHERE A.id=X.kayttaja_id AND B.id=Y.kayttaja_id AND X.ryhma_id=Y.ryhma_id AND B.tunnus='uolevi';
```

---



## Tehtävä 65 
Hae kaikki käyttäjät, jotka eivät kuulu mihinkään samaan ryhmään käyttäjän "uolevi" kanssa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Kayttajat</i><table border=""><tbody><tr><th>id</th><th>tunnus</th></tr><tr><td>1</td><td>uolevi</td></tr><tr><td>2</td><td>maija</td></tr><tr><td>3</td><td>kaaleppi</td></tr><tr><td>4</td><td>liisa</td></tr></tbody></table></td><td width="20"></td><td><i>Ryhmat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>puput</td></tr><tr><td>2</td><td>kilit</td></tr></tbody></table></td><td width="20"></td><td><i>Oikeudet</i><table border=""><tbody><tr><th>kayttaja_id</th><th>ryhma_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>1</td><td>2</td></tr><tr><td>2</td><td>1</td></tr><tr><td>4</td><td>2</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>kaaleppi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Kayttajat.tunnus FROM Kayttajat WHERE Kayttajat.id
NOT IN (SELECT Oikeudet.kayttaja_id FROM Oikeudet WHERE Oikeudet.ryhma_id
  IN (SELECT Oikeudet.ryhma_id FROM Oikeudet, Kayttajat WHERE Oikeudet.kayttaja_id == 1));
```
#### Mallivastaus
```sql
SELECT tunnus FROM Kayttajat WHERE tunnus NOT IN (SELECT A.tunnus FROM Kayttajat A, Kayttajat B, Oikeudet X, Oikeudet Y WHERE A.id=X.kayttaja_id AND B.id=Y.kayttaja_id AND X.ryhma_id=Y.ryhma_id AND B.tunnus='uolevi');
```

---



## Tehtävä 66 
Hae sanat järjestettynä niin, että kirjainkoolla ei ole merkitystä. Jokainen sana muodostuu kirjaimista a–z ja A–Z.

**Taulut**

<table><tbody><tr valign="top"><td><i>Sanat</i><table border=""><tbody><tr><th>id</th><th>sana</th></tr><tr><td>1</td><td>Liisa</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Uolevi</td></tr><tr><td>4</td><td>apina</td></tr><tr><td>5</td><td>omena</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>apina</td></tr><tr><td>Liisa</td></tr><tr><td>Maija</td></tr><tr><td>omena</td></tr><tr><td>Uolevi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT sana FROM Sanat ORDER BY LOWER(sana);
```
#### Mallivastaus
```sql
SELECT sana FROM Sanat ORDER BY LOWER(sana);
```

---



## Tehtävä 67 
Hae tuote, jonka hinta on halvin (jos halvimpia tuotteita on useita, valitse aakkosjärjestyksessä ensimmäinen).

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>5</td></tr><tr><td>3</td><td>retiisi</td><td>8</td></tr><tr><td>4</td><td>nauris</td><td>5</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>lanttu</td><td>5</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi, Tuotteet.hinta
FROM Tuotteet
WHERE Tuotteet.hinta =
(SELECT MIN
 (Tuotteet.hinta)
 FROM Tuotteet
 GROUP BY hinta)
ORDER BY nimi
LIMIT 1;
```
#### Mallivastaus
```sql
SELECT nimi, hinta FROM Tuotteet ORDER BY hinta, nimi LIMIT 1;
```

---



## Tehtävä 68 
Hae jokaisesta tuotteesta tieto, monenko tuotteen hinta eroaa enintään yhdellä (tässä lasketaan mukaan myös tuote itse).

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>4</td></tr><tr><td>3</td><td>retiisi</td><td>8</td></tr><tr><td>4</td><td>nauris</td><td>6</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>selleri</td><td>3</td></tr><tr><td>lanttu</td><td>1</td></tr><tr><td>retiisi</td><td>2</td></tr><tr><td>nauris</td><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi, COUNT(*)
  FROM Tuotteet, Tuotteet t3
  WHERE Tuotteet.id IN (SELECT t2.id 
     FROM Tuotteet t2 WHERE ABS(Tuotteet.hinta-t3.hinta) <=1)
GROUP BY Tuotteet.nimi;
```
#### Mallivastaus
```sql
SELECT A.nimi, COUNT(*) FROM Tuotteet A, Tuotteet B WHERE ABS(A.hinta-B.hinta) <= 1 GROUP BY A.id;
```

---



## Tehtävä 69 
Laske, monellako tavalla voit valita kaksi tuotetta niin, että yhteishinta on tasan 10.

Huom! Yhdistelmässä voi olla kaksi samaa tuotetta ja halutaan laskea erilaiset yhdistelmät. Esimerkissä yhdistelmät ovat selleri+selleri ja lanttu+nauris (eli nauris+lanttu ei ole mukana).

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>5</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>8</td></tr><tr><td>4</td><td>nauris</td><td>7</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT COUNT(n1)
FROM
(
 SELECT t1.nimi n1, t2.nimi n2
 FROM Tuotteet t1, Tuotteet t2
 WHERE t1.hinta + t2.hinta == 10
 AND t1.nimi <= t2.nimi
);
```
#### Mallivastaus
```sql
SELECT COUNT(*) FROM Tuotteet A, Tuotteet B WHERE A.hinta+B.hinta=10 AND A.id <= B.id;
```

---



## Tehtävä 70 
Laske, mikä on pienin ero kahden tuotteen hinnassa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>5</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>8</td></tr><tr><td>4</td><td>nauris</td><td>7</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT MIN(ABS(hinta1 - hinta2)) 
FROM (SELECT t1.id AS id1, t2.id AS id2, t1.hinta AS hinta1, t2.hinta AS hinta2 
   FROM Tuotteet t1, Tuotteet t2 
   WHERE id1!=id2);
```
#### Mallivastaus
```sql
SELECT MIN(ABS(A.hinta-B.hinta)) FROM Tuotteet A, Tuotteet B WHERE A.id<>B.id;
```

---



## Tehtävä 71 
Laske jokaisen tilin saldo tapahtumien perusteella (jokaisen tilin saldo on aluksi 0).

**Taulut**

<table><tbody><tr valign="top"><td><i>Tilit</i><table border=""><tbody><tr><th>id</th><th>haltija</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tapahtumat</i><table border=""><tbody><tr><th>id</th><th>tili_id</th><th>muutos</th></tr><tr><td>1</td><td>1</td><td>500</td></tr><tr><td>2</td><td>2</td><td>300</td></tr><tr><td>3</td><td>1</td><td>-100</td></tr><tr><td>4</td><td>2</td><td>100</td></tr><tr><td>5</td><td>2</td><td>-300</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>400</td></tr><tr><td>Maija</td><td>100</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT haltija, COALESCE(tilisumma, 0) FROM (SELECT Tilit.haltija, tilisumma FROM (Tilit LEFT JOIN (SELECT t1.tili_id AS tili1, SUM(t1.muutos) AS tilisumma FROM Tapahtumat t1 GROUP BY t1.tili_id) ON Tilit.id = tili1) GROUP BY Tilit.id);
```
#### Mallivastaus
```sql
SELECT A.haltija, IFNULL(SUM(B.muutos),0) FROM Tilit A LEFT JOIN Tapahtumat B ON A.id=B.tili_id GROUP BY A.id;
```

---



## Tehtävä 72 
Laske Uolevin tilin saldon historia. Tapahtumat ovat järjestyksessä id:n mukaisesti.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tilit</i><table border=""><tbody><tr><th>id</th><th>haltija</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tapahtumat</i><table border=""><tbody><tr><th>id</th><th>tili_id</th><th>muutos</th></tr><tr><td>1</td><td>1</td><td>500</td></tr><tr><td>2</td><td>2</td><td>300</td></tr><tr><td>3</td><td>1</td><td>-100</td></tr><tr><td>4</td><td>2</td><td>100</td></tr><tr><td>5</td><td>2</td><td>-300</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>500</td></tr><tr><td>400</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT SUM(Tapahmtos) 
OVER ( ORDER BY TapahID ) 
FROM (SELECT Tapahtumat.id AS tapahID, Tapahtumat.muutos AS Tapahmtos 
    FROM Tapahtumat, Tilit 
    WHERE Tilit.id = Tapahtumat.tili_id 
    AND Tilit.haltija = 'Uolevi');
```
#### Mallivastaus
```sql
SELECT SUM(B.muutos) FROM Tilit T, Tapahtumat A, Tapahtumat B WHERE A.tili_id=T.id AND B.tili_id=T.id AND T.haltija="Uolevi" AND B.id<=A.id GROUP BY A.id;
```

---



## Tehtävä 73 
Laske jokaisen tilin suurin saldo historian aikana (jokaisen tilin saldo on aluksi 0).

**Taulut**

<table><tbody><tr valign="top"><td><i>Tilit</i><table border=""><tbody><tr><th>id</th><th>haltija</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tapahtumat</i><table border=""><tbody><tr><th>id</th><th>tili_id</th><th>muutos</th></tr><tr><td>1</td><td>1</td><td>500</td></tr><tr><td>2</td><td>2</td><td>300</td></tr><tr><td>3</td><td>1</td><td>-100</td></tr><tr><td>4</td><td>2</td><td>100</td></tr><tr><td>5</td><td>2</td><td>-300</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>500</td></tr><tr><td>Maija</td><td>400</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT haltija, MAX(tili) FROM (SELECT Tilit.haltija haltija, COALESCE(SUM(taph2.muutos),0) tili
FROM Tilit LEFT JOIN Tapahtumat taph1 ON Tilit.id = taph1.tili_id
LEFT JOIN Tapahtumat taph2 ON taph2.id <= taph1.id AND Tilit.id = taph2.tili_id GROUP BY taph1.id, haltija ORDER BY tili DESC) GROUP BY haltija ORDER BY tili DESC;
```
#### Mallivastaus
```sql
SELECT haltija, IFNULL((SELECT MAX((SELECT SUM(muutos) FROM Tapahtumat WHERE tili_id=B.id AND id <= A.id)) FROM Tapahtumat A),0) FROM Tilit B;
```

---



## Tehtävä 74 
Laske, montako eri tehtävää kukin opiskelija on ratkaissut oikein (lähetyksen tila on 0 = väärin tai 1 = oikein).

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tehtavat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>T1</td></tr><tr><td>2</td><td>T2</td></tr><tr><td>3</td><td>T3</td></tr></tbody></table></td><td width="20"></td><td><i>Lahetykset</i><table border=""><tbody><tr><th>id</th><th>opiskelija_id</th><th>tehtava_id</th><th>tila</th></tr><tr><td>1</td><td>1</td><td>1</td><td>0</td></tr><tr><td>2</td><td>1</td><td>1</td><td>0</td></tr><tr><td>3</td><td>2</td><td>1</td><td>1</td></tr><tr><td>4</td><td>1</td><td>2</td><td>0</td></tr><tr><td>5</td><td>1</td><td>1</td><td>1</td></tr><tr><td>6</td><td>2</td><td>2</td><td>1</td></tr><tr><td>7</td><td>2</td><td>3</td><td>0</td></tr><tr><td>8</td><td>1</td><td>2</td><td>0</td></tr><tr><td>9</td><td>1</td><td>2</td><td>1</td></tr><tr><td>10</td><td>2</td><td>2</td><td>1</td></tr><tr><td>11</td><td>2</td><td>2</td><td>1</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>2</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, COUNT(DISTINCT Lahetykset.tehtava_id)
FROM Opiskelijat LEFT JOIN Lahetykset ON (Opiskelijat.id = Lahetykset.opiskelija_id
AND Lahetykset.tila=1) GROUP BY Opiskelijat.id;
```
#### Mallivastaus
```sql
SELECT O.nimi, COUNT(DISTINCT L.tehtava_id) FROM Opiskelijat O LEFT JOIN Lahetykset L ON O.id=L.opiskelija_id AND L.tila=1 GROUP BY O.id;
```

---



## Tehtävä 75 
Laske jokaiselle opiskelijalle, montako lähetystä enimmillään hän on lähettänyt samaan tehtävään.

**Taulut**

<table><tbody><tr valign="top"><td><i>Opiskelijat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tehtavat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>T1</td></tr><tr><td>2</td><td>T2</td></tr><tr><td>3</td><td>T3</td></tr></tbody></table></td><td width="20"></td><td><i>Lahetykset</i><table border=""><tbody><tr><th>id</th><th>opiskelija_id</th><th>tehtava_id</th><th>tila</th></tr><tr><td>1</td><td>1</td><td>1</td><td>0</td></tr><tr><td>2</td><td>2</td><td>1</td><td>1</td></tr><tr><td>3</td><td>1</td><td>2</td><td>0</td></tr><tr><td>4</td><td>1</td><td>1</td><td>1</td></tr><tr><td>5</td><td>2</td><td>2</td><td>1</td></tr><tr><td>6</td><td>2</td><td>3</td><td>0</td></tr><tr><td>7</td><td>1</td><td>2</td><td>0</td></tr><tr><td>8</td><td>2</td><td>2</td><td>1</td></tr><tr><td>9</td><td>2</td><td>2</td><td>1</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>2</td></tr><tr><td>Maija</td><td>3</td></tr><tr><td>Kaaleppi</td><td>0</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Opiskelijat.nimi, COALESCE((SELECT COUNT(Lahetykset.tehtava_id) tulos FROM Lahetykset, Tehtavat WHERE 
Lahetykset.opiskelija_id = Opiskelijat.id AND Lahetykset.tehtava_id = Tehtavat.id GROUP BY Lahetykset.tehtava_id ORDER BY tulos DESC), 0) FROM Opiskelijat;
```
#### Mallivastaus
```sql
SELECT nimi, IFNULL((SELECT MAX(maara) FROM (SELECT COUNT(*) maara FROM Lahetykset WHERE opiskelija_id=O.id GROUP BY tehtava_id)),0) FROM Opiskelijat O;
```

---



## Tehtävä 76 
Laske tulosten moodi (eli yleisin tulos). Jos vaihtoehtoja on useita, valitse niistä pienin.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>tulos</th></tr><tr><td>1</td><td>2</td></tr><tr><td>2</td><td>2</td></tr><tr><td>3</td><td>3</td></tr><tr><td>4</td><td>5</td></tr><tr><td>5</td><td>5</td></tr><tr><td>6</td><td>5</td></tr><tr><td>7</td><td>6</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>5</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT tulos
FROM Tulokset
GROUP BY Tulokset.tulos
ORDER BY COUNT(*) DESC, tulos ASC LIMIT 1;
```
#### Mallivastaus
```sql
SELECT tulos FROM Tulokset GROUP BY tulos ORDER BY COUNT(*) DESC, tulos LIMIT 1;
```

---



## Tehtävä 77 
Laske tulosten mediaani (eli keskimmäinen tulos, kun tulokset on järjestetty pienimmästä suurimpaan). Voit olettaa, että tulosten määrä on pariton.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>tulos</th></tr><tr><td>1</td><td>5</td></tr><tr><td>2</td><td>2</td></tr><tr><td>3</td><td>3</td></tr><tr><td>4</td><td>5</td></tr><tr><td>5</td><td>2</td></tr><tr><td>6</td><td>6</td></tr><tr><td>7</td><td>5</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>5</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tulokset.tulos FROM Tulokset ORDER BY tulos LIMIT 1
OFFSET (SELECT COUNT(*) FROM Tulokset) / 2;
```
#### Mallivastaus
```sql
SELECT tulos FROM Tulokset ORDER BY tulos LIMIT 1 OFFSET (SELECT COUNT(*)/2 FROM Tulokset);
```

---



## Tehtävä 78 
Laske tulosten mediaani (eli keskimmäinen tulos, kun tulokset on järjestetty pienimmästä suurimpaan). Jos tulosten määrä on parillinen, tulosta keskikohdan vasemmalla puolella oleva tulos.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>tulos</th></tr><tr><td>1</td><td>3</td></tr><tr><td>2</td><td>2</td></tr><tr><td>3</td><td>7</td></tr><tr><td>4</td><td>3</td></tr><tr><td>5</td><td>4</td></tr><tr><td>6</td><td>7</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>3</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT x.tulos FROM (SELECT tulos, COUNT(1) OVER (partition BY 'A') AS TotalRows, Row_number()
OVER (ORDER BY Tulos aSC) AS AmountOrder FROM Tulokset ft) x 
WHERE x.AmountOrder = ROUND(x.TotalRows / 2.0, 0);
```
#### Mallivastaus
```sql
SELECT tulos FROM Tulokset ORDER BY tulos LIMIT 1 OFFSET (SELECT (COUNT(*)-1)/2 FROM Tulokset);
```

---



## Tehtävä 79 
Ilmoita jokaisesta junan vaunusta, montako matkustajaa siellä on.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>vaunu1</td><td>2</td></tr><tr><td>vaunu2</td><td>1</td></tr><tr><td>vaunu3</td><td>0</td></tr><tr><td>vaunu4</td><td>3</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Vaunut.nimi,
(
 SELECT COUNT(Matkustajat.vaunu_id)
 FROM Matkustajat
WHERE Matkustajat.vaunu_id = Vaunut.id
)
  FROM Vaunut;
```
#### Mallivastaus
```sql
SELECT V.nimi, COUNT(M.id) FROM Vaunut V LEFT JOIN Matkustajat M ON V.id=M.vaunu_id GROUP BY V.id;
```

---



## Tehtävä 80 
Ilmoita jokaisesta junan vaunusta, montako tyhjää paikkaa siellä on.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>vaunu1</td><td>8</td></tr><tr><td>vaunu2</td><td>9</td></tr><tr><td>vaunu3</td><td>10</td></tr><tr><td>vaunu4</td><td>7</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Vaunut.nimi, (Vaunut.paikat - (SELECT COUNT(Matkustajat.vaunu_id) FROM Matkustajat
WHERE Matkustajat.vaunu_id = Vaunut.id)) FROM Vaunut;
```
#### Mallivastaus
```sql
SELECT V.nimi, V.paikat-COUNT(M.id) FROM Vaunut V LEFT JOIN Matkustajat M ON V.id=M.vaunu_id GROUP BY V.id;
```

---



## Tehtävä 81 
Laske, montako tyhjää paikkaa junassa on kaikkiaan.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>34</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT SUM(Vaunut.paikat - (SELECT COUNT(Matkustajat.vaunu_id) FROM Matkustajat
WHERE Matkustajat.vaunu_id = Vaunut.id)) FROM Vaunut;
```
#### Mallivastaus
```sql
SELECT (SELECT SUM(paikat) FROM vaunut)-(SELECT COUNT(*) FROM Matkustajat);
```

---



## Tehtävä 82 
Hae jokaisesta matkustajasta tieto, montako muuta matkustajaa on samassa vaunussa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Uolevi</td><td>1</td></tr><tr><td>Maija</td><td>1</td></tr><tr><td>Kaaleppi</td><td>0</td></tr><tr><td>Kotivalo</td><td>2</td></tr><tr><td>Justiina</td><td>2</td></tr><tr><td>Vihtori</td><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi, COUNT(n1) FROM Matkustajat LEFT JOIN (SELECT m1.nimi AS n1, m2.nimi AS n2
FROM Matkustajat m1, Matkustajat m2 WHERE (m1.vaunu_id=m2.vaunu_id AND m1.nimi != m2.nimi)) ON nimi=n1 GROUP BY n1 ORDER BY id;
```
#### Mallivastaus
```sql
SELECT A.nimi, COUNT(*)-1 FROM Matkustajat A, Matkustajat B WHERE A.vaunu_id=B.vaunu_id GROUP BY A.id;
```

---



## Tehtävä 83 
Hae kaikki matkustajat, jotka ovat yksin vaunussaan.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Kaaleppi</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT A.nimi FROM Matkustajat A, Matkustajat B WHERE A.vaunu_id=B.vaunu_id GROUP BY A.id HAVING COUNT(*)-1 = 0;
```
#### Mallivastaus
```sql
SELECT A.nimi FROM Matkustajat A, Matkustajat B WHERE A.vaunu_id=B.vaunu_id GROUP BY A.id HAVING COUNT(*)=1;
```

---



## Tehtävä 84 
Hae kaikki vaunut, joissa ei ole yhtään matkustajaa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>vaunu3</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Vaunut.nimi FROM Vaunut WHERE((SELECT COUNT(*) FROM Matkustajat 
WHERE Vaunut.id = Matkustajat.vaunu_id) == 0);
```
#### Mallivastaus
```sql
SELECT V.nimi FROM Vaunut V LEFT JOIN Matkustajat M ON V.id=M.vaunu_id GROUP BY V.id HAVING COUNT(M.id)=0;
```

---



## Tehtävä 85 
Laske, monellako tavalla voidaan valita kaksi matkustajaa, jotka ovat samassa vaunussa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Vaunut</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>paikat</th></tr><tr><td>1</td><td>vaunu1</td><td>10</td></tr><tr><td>2</td><td>vaunu2</td><td>10</td></tr><tr><td>3</td><td>vaunu3</td><td>10</td></tr><tr><td>4</td><td>vaunu4</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Matkustajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>vaunu_id</th></tr><tr><td>1</td><td>Uolevi</td><td>1</td></tr><tr><td>2</td><td>Maija</td><td>1</td></tr><tr><td>3</td><td>Kaaleppi</td><td>2</td></tr><tr><td>4</td><td>Kotivalo</td><td>4</td></tr><tr><td>5</td><td>Justiina</td><td>4</td></tr><tr><td>6</td><td>Vihtori</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>4</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT COUNT(*)/2 FROM (SELECT M1.nimi, M2.nimi FROM Matkustajat M1, Matkustajat
 M2 WHERE M1.vaunu_id = M2.vaunu_id AND M1.nimi != M2.nimi);
```
#### Mallivastaus
```sql
SELECT COUNT(*) FROM Matkustajat A, Matkustajat B WHERE A.id<B.id AND A.vaunu_id=B.vaunu_id;
```

---



## Tehtävä 86 
Hae jokaisesta paketista tuotteiden määrä ja eri tuotteiden määrä.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>5</td></tr><tr><td>4</td><td>nauris</td><td>6</td></tr></tbody></table></td><td width="20"></td><td><i>Paketit</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>Mummon herkut</td><td>10</td></tr><tr><td>2</td><td>Kolmikko</td><td>14</td></tr></tbody></table></td><td width="20"></td><td><i>Sisallot</i><table border=""><tbody><tr><th>paketti_id</th><th>tuote_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>1</td><td>4</td></tr><tr><td>2</td><td>3</td></tr><tr><td>2</td><td>3</td></tr><tr><td>2</td><td>3</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Mummon herkut</td><td>2</td><td>2</td></tr><tr><td>Kolmikko</td><td>3</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT asetelma.nimi, COUNT(asetelma.tuote_id), COUNT(DISTINCT asetelma.tuote_id)
FROM (Paketit 
LEFT JOIN Sisallot 
ON Paketit.id = Sisallot.paketti_id) asetelma 
GROUP BY asetelma.nimi;
```
#### Mallivastaus
```sql
SELECT P.nimi, COUNT(S.tuote_id), COUNT(DISTINCT S.tuote_id) FROM Paketit P LEFT JOIN Sisallot S ON P.id=S.paketti_id GROUP BY P.id;
```

---



## Tehtävä 89 
Hae jokaisesta tuotteesta tieto, montako kertaa se esiintyy enimmillään samassa paketissa.

**Taulut**

<table><tbody><tr valign="top"><td><i>Tuotteet</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>selleri</td><td>7</td></tr><tr><td>2</td><td>lanttu</td><td>3</td></tr><tr><td>3</td><td>retiisi</td><td>5</td></tr><tr><td>4</td><td>nauris</td><td>6</td></tr></tbody></table></td><td width="20"></td><td><i>Paketit</i><table border=""><tbody><tr><th>id</th><th>nimi</th><th>hinta</th></tr><tr><td>1</td><td>Mummon herkut</td><td>10</td></tr><tr><td>2</td><td>Papan herkut</td><td>10</td></tr></tbody></table></td><td width="20"></td><td><i>Sisallot</i><table border=""><tbody><tr><th>paketti_id</th><th>tuote_id</th></tr><tr><td>1</td><td>1</td></tr><tr><td>1</td><td>4</td></tr><tr><td>2</td><td>3</td></tr><tr><td>2</td><td>3</td></tr><tr><td>2</td><td>4</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>selleri</td><td>1</td></tr><tr><td>lanttu</td><td>0</td></tr><tr><td>retiisi</td><td>2</td></tr><tr><td>nauris</td><td>1</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT Tuotteet.nimi, COALESCE((SELECT COUNT(*) tulos FROM Sisallot, Paketit WHERE 
Sisallot.paketti_id = Paketit.id AND Sisallot.tuote_id = Tuotteet.id GROUP BY Sisallot.paketti_id ORDER BY Sisallot.paketti_id DESC), 0) FROM Tuotteet;
```
#### Mallivastaus
```sql
SELECT nimi, IFNULL((SELECT MAX(maara) FROM (SELECT COUNT(*) maara FROM Sisallot WHERE tuote_id=T.id GROUP BY paketti_id)),0) FROM Tuotteet T;
```

---



## Tehtävä 90 
Muodosta tuloslista, jossa on sijaluku, pelaajan nimi ja paras tulos. Jos kahdella pelaajalla on sama tulos, nimet järjestetään aakkosjärjestykseen. Jokaisella pelaajalla on eri nimi ja ainakin yksi tulos.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Kaaleppi</td></tr></tbody></table></td><td width="20"></td><td><i>Tulokset</i><table border=""><tbody><tr><th>id</th><th>pelaaja_id</th><th>tulos</th></tr><tr><td>1</td><td>1</td><td>100</td></tr><tr><td>2</td><td>1</td><td>350</td></tr><tr><td>3</td><td>2</td><td>300</td></tr><tr><td>4</td><td>2</td><td>350</td></tr><tr><td>5</td><td>3</td><td>500</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>1</td><td>Kaaleppi</td><td>500</td></tr><tr><td>2</td><td>Maija</td><td>350</td></tr><tr><td>3</td><td>Uolevi</td><td>350</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT RANK() OVER (ORDER BY Pelaajat.nimi ASC), Pelaajat.nimi, MAX(tulos) FROM Tulokset, Pelaajat WHERE pelaaja_id=Pelaajat.id GROUP BY Pelaajat.id;
```
#### Mallivastaus
```sql
SELECT ROW_NUMBER() OVER (ORDER BY MAX(T.tulos) DESC, P.nimi), P.nimi, MAX(T.tulos) FROM Pelaajat P, Tulokset T WHERE P.id=T.pelaaja_id GROUP BY P.id;
```

---



## Tehtävä 96 
Pelaajat jaetaan joukkueisiin niin, että aakkosjärjestyksessä joka toinen pelaaja kuuluu joukkueeseen 1 ja 2. Ilmoita joukkuejako annetuille pelaajille.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Liisa</td></tr><tr><td>4</td><td>Kaaleppi</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Kaaleppi</td><td>1</td></tr><tr><td>Liisa</td><td>2</td></tr><tr><td>Maija</td><td>1</td></tr><tr><td>Uolevi</td><td>2</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi, ((ROW_NUMBER() OVER (ORDER BY nimi)) - 1) % 2 +1 AS rivi FROM Pelaajat ORDER BY nimi;
```
#### Mallivastaus
```sql
SELECT nimi, 2-(ROW_NUMBER() OVER (ORDER BY nimi))%2 FROM Pelaajat;
```

---



## Tehtävä 97 
Pelaajat jaetaan joukkueisiin niin, että aakkosjärjestyksessä joka toinen pelaaja kuuluu joukkueeseen "Puput" ja "Kilit". Ilmoita joukkuejako annetuille pelaajille.

**Taulut**

<table><tbody><tr valign="top"><td><i>Pelaajat</i><table border=""><tbody><tr><th>id</th><th>nimi</th></tr><tr><td>1</td><td>Uolevi</td></tr><tr><td>2</td><td>Maija</td></tr><tr><td>3</td><td>Liisa</td></tr><tr><td>4</td><td>Kaaleppi</td></tr></tbody></table></td></tr></tbody></table>

  

**Haluttu tulos**

<table border=""><tbody><tr><td>Kaaleppi</td><td>Puput</td></tr><tr><td>Liisa</td><td>Kilit</td></tr><tr><td>Maija</td><td>Puput</td></tr><tr><td>Uolevi</td><td>Kilit</td></tr></tbody></table>

#### Vastauksesi 
```sql
SELECT nimi, CASE ((ROW_NUMBER() OVER (ORDER BY nimi)) - 1) % 2 +1 WHEN 1 THEN 'Puput' WHEN 2 THEN 'Kilit' END FROM Pelaajat ORDER BY nimi;
```
#### Mallivastaus
```sql
SELECT nimi, CASE WHEN (ROW_NUMBER() OVER (ORDER BY nimi))%2=1 THEN 'Puput' ELSE 'Kilit' END FROM Pelaajat;
```

---
