# SQL_HW
```
 use world
Database changed
mysql> show tables;
+-----------------+
| Tables_in_world |
+-----------------+
| city            |
| country         |
| countrylanguage |
+-----------------+
3 rows in set (0.00 sec)

mysql> Select COUNT(*) AS cities from city where CountryCode='USA';
+--------+
| cities |
+--------+
|    274 |
+--------+
1 row in set (0.02 sec)

mysql> Select Population, AVG(LifeExpectancy) from country where Code ='ARG';
+------------+---------------------+
| Population | AVG(LifeExpectancy) |
+------------+---------------------+
|   37032000 |            75.10000 |
+------------+---------------------+
1 row in set (0.03 sec)

mysql> select * from city where CountryCode='JPN';
+------+---------------------+-------------+-----------+------------+
| ID   | Name                | CountryCode | District  | Population |
+------+---------------------+-------------+-----------+------------+
| 1532 | Tokyo               | JPN         | Tokyo-to  |    7980230 |
| 1533 | Jokohama [Yokohama] | JPN         | Kanagawa  |    3339594 |
| 1534 | Osaka               | JPN         | Osaka     |    2595674 |
| 1535 | Nagoya              | JPN         | Aichi     |    2154376 |
| 1536 | Sapporo             | JPN         | Hokkaido  |    1790886 |
| 1537 | Kioto               | JPN         | Kyoto     |    1461974 |
| 1538 | Kobe                | JPN         | Hyogo     |    1425139 |
| 1539 | Fukuoka             | JPN         | Fukuoka   |    1308379 |
| 1540 | Kawasaki            | JPN         | Kanagawa  |    1217359 |
| 1541 | Hiroshima           | JPN         | Hiroshima |    1119117 |
| 1542 | Kitakyushu          | JPN         | Fukuoka   |    1016264 |
| 1543 | Sendai              | JPN         | Miyagi    |     989975 |
| 1544 | Chiba               | JPN         | Chiba     |     863930 |
| 1545 | Sakai               | JPN         | Osaka     |     797735 |
| 1546 | Kumamoto            | JPN         | Kumamoto  |     656734 |
| 1547 | Okayama             | JPN         | Okayama   |     624269 |
| 1548 | Sagamihara          | JPN         | Kanagawa  |     586300 |
| 1549 | Hamamatsu           | JPN         | Shizuoka  |     568796 |
| 1550 | Kagoshima           | JPN         | Kagoshima |     549977 |
| 1551 | Funabashi           | JPN         | Chiba     |     545299 |
| 1552 | Higashiosaka        | JPN         | Osaka     |     517785 |
| 1553 | Hachioji            | JPN         | Tokyo-to  |     513451 |
| 1554 | Niigata             | JPN         | Niigata   |     497464 |
| 1555 | Amagasaki           | JPN         | Hyogo     |     481434 |
| 1556 | Himeji              | JPN         | Hyogo     |     475167 |
| 1557 | Shizuoka            | JPN         | Shizuoka  |     473854 |
| 1558 | Urawa               | JPN         | Saitama   |     469675 |
| 1559 | Matsuyama           | JPN         | Ehime     |     466133 |
| 1560 | Matsudo             | JPN         | Chiba     |     461126 |
| 1561 | Kanazawa            | JPN         | Ishikawa  |     455386 |
| 1562 | Kawaguchi           | JPN         | Saitama   |     452155 |
| 1563 | Ichikawa            | JPN         | Chiba     |     441893 |
| 1564 | Omiya               | JPN         | Saitama   |     441649 |
| 1565 | Utsunomiya          | JPN         | Tochigi   |     440353 |
| 1566 | Oita                | JPN         | Oita      |     433401 |
| 1567 | Nagasaki            | JPN         | Nagasaki  |     432759 |
| 1568 | Yokosuka            | JPN         | Kanagawa  |     430200 |
| 1569 | Kurashiki           | JPN         | Okayama   |     425103 |
| 1570 | Gifu                | JPN         | Gifu      |     408007 |
| 1571 | Hirakata            | JPN         | Osaka     |     403151 |
| 1572 | Nishinomiya         | JPN         | Hyogo     |     397618 |
| 1573 | Toyonaka            | JPN         | Osaka     |     396689 |
| 1574 | Wakayama            | JPN         | Wakayama  |     391233 |
| 1575 | Fukuyama            | JPN         | Hiroshima |     376921 |
| 1576 | Fujisawa            | JPN         | Kanagawa  |     372840 |
| 1577 | Asahikawa           | JPN         | Hokkaido  |     364813 |
| 1578 | Machida             | JPN         | Tokyo-to  |     364197 |
| 1579 | Nara                | JPN         | Nara      |     362812 |
| 1580 | Takatsuki           | JPN         | Osaka     |     361747 |
| 1581 | Iwaki               | JPN         | Fukushima |     361737 |
| 1582 | Nagano              | JPN         | Nagano    |     361391 |
| 1583 | Toyohashi           | JPN         | Aichi     |     360066 |
| 1584 | Toyota              | JPN         | Aichi     |     346090 |
| 1585 | Suita               | JPN         | Osaka     |     345750 |
| 1586 | Takamatsu           | JPN         | Kagawa    |     332471 |
| 1587 | Koriyama            | JPN         | Fukushima |     330335 |
| 1588 | Okazaki             | JPN         | Aichi     |     328711 |
| 1589 | Kawagoe             | JPN         | Saitama   |     327211 |
| 1590 | Tokorozawa          | JPN         | Saitama   |     325809 |
| 1591 | Toyama              | JPN         | Toyama    |     325790 |
| 1592 | Kochi               | JPN         | Kochi     |     324710 |
| 1593 | Kashiwa             | JPN         | Chiba     |     320296 |
| 1594 | Akita               | JPN         | Akita     |     314440 |
| 1595 | Miyazaki            | JPN         | Miyazaki  |     303784 |
| 1596 | Koshigaya           | JPN         | Saitama   |     301446 |
| 1597 | Naha                | JPN         | Okinawa   |     299851 |
| 1598 | Aomori              | JPN         | Aomori    |     295969 |
| 1599 | Hakodate            | JPN         | Hokkaido  |     294788 |
| 1600 | Akashi              | JPN         | Hyogo     |     292253 |
| 1601 | Yokkaichi           | JPN         | Mie       |     288173 |
| 1602 | Fukushima           | JPN         | Fukushima |     287525 |
| 1603 | Morioka             | JPN         | Iwate     |     287353 |
| 1604 | Maebashi            | JPN         | Gumma     |     284473 |
| 1605 | Kasugai             | JPN         | Aichi     |     282348 |
| 1606 | Otsu                | JPN         | Shiga     |     282070 |
| 1607 | Ichihara            | JPN         | Chiba     |     279280 |
| 1608 | Yao                 | JPN         | Osaka     |     276421 |
| 1609 | Ichinomiya          | JPN         | Aichi     |     270828 |
| 1610 | Tokushima           | JPN         | Tokushima |     269649 |
| 1611 | Kakogawa            | JPN         | Hyogo     |     266281 |
| 1612 | Ibaraki             | JPN         | Osaka     |     261020 |
| 1613 | Neyagawa            | JPN         | Osaka     |     257315 |
| 1614 | Shimonoseki         | JPN         | Yamaguchi |     257263 |
| 1615 | Yamagata            | JPN         | Yamagata  |     255617 |
| 1616 | Fukui               | JPN         | Fukui     |     254818 |
| 1617 | Hiratsuka           | JPN         | Kanagawa  |     254207 |
| 1618 | Mito                | JPN         | Ibaragi   |     246559 |
| 1619 | Sasebo              | JPN         | Nagasaki  |     244240 |
| 1620 | Hachinohe           | JPN         | Aomori    |     242979 |
| 1621 | Takasaki            | JPN         | Gumma     |     239124 |
| 1622 | Shimizu             | JPN         | Shizuoka  |     239123 |
| 1623 | Kurume              | JPN         | Fukuoka   |     235611 |
| 1624 | Fuji                | JPN         | Shizuoka  |     231527 |
| 1625 | Soka                | JPN         | Saitama   |     222768 |
| 1626 | Fuchu               | JPN         | Tokyo-to  |     220576 |
| 1627 | Chigasaki           | JPN         | Kanagawa  |     216015 |
| 1628 | Atsugi              | JPN         | Kanagawa  |     212407 |
| 1629 | Numazu              | JPN         | Shizuoka  |     211382 |
| 1630 | Ageo                | JPN         | Saitama   |     209442 |
| 1631 | Yamato              | JPN         | Kanagawa  |     208234 |
| 1632 | Matsumoto           | JPN         | Nagano    |     206801 |
| 1633 | Kure                | JPN         | Hiroshima |     206504 |
| 1634 | Takarazuka          | JPN         | Hyogo     |     205993 |
| 1635 | Kasukabe            | JPN         | Saitama   |     201838 |
| 1636 | Chofu               | JPN         | Tokyo-to  |     201585 |
| 1637 | Odawara             | JPN         | Kanagawa  |     200171 |
| 1638 | Kofu                | JPN         | Yamanashi |     199753 |
| 1639 | Kushiro             | JPN         | Hokkaido  |     197608 |
| 1640 | Kishiwada           | JPN         | Osaka     |     197276 |
| 1641 | Hitachi             | JPN         | Ibaragi   |     196622 |
| 1642 | Nagaoka             | JPN         | Niigata   |     192407 |
| 1643 | Itami               | JPN         | Hyogo     |     190886 |
| 1644 | Uji                 | JPN         | Kyoto     |     188735 |
| 1645 | Suzuka              | JPN         | Mie       |     184061 |
| 1646 | Hirosaki            | JPN         | Aomori    |     177522 |
| 1647 | Ube                 | JPN         | Yamaguchi |     175206 |
| 1648 | Kodaira             | JPN         | Tokyo-to  |     174984 |
| 1649 | Takaoka             | JPN         | Toyama    |     174380 |
| 1650 | Obihiro             | JPN         | Hokkaido  |     173685 |
| 1651 | Tomakomai           | JPN         | Hokkaido  |     171958 |
| 1652 | Saga                | JPN         | Saga      |     170034 |
| 1653 | Sakura              | JPN         | Chiba     |     168072 |
| 1654 | Kamakura            | JPN         | Kanagawa  |     167661 |
| 1655 | Mitaka              | JPN         | Tokyo-to  |     167268 |
| 1656 | Izumi               | JPN         | Osaka     |     166979 |
| 1657 | Hino                | JPN         | Tokyo-to  |     166770 |
| 1658 | Hadano              | JPN         | Kanagawa  |     166512 |
| 1659 | Ashikaga            | JPN         | Tochigi   |     165243 |
| 1660 | Tsu                 | JPN         | Mie       |     164543 |
| 1661 | Sayama              | JPN         | Saitama   |     162472 |
| 1662 | Yachiyo             | JPN         | Chiba     |     161222 |
| 1663 | Tsukuba             | JPN         | Ibaragi   |     160768 |
| 1664 | Tachikawa           | JPN         | Tokyo-to  |     159430 |
| 1665 | Kumagaya            | JPN         | Saitama   |     157171 |
| 1666 | Moriguchi           | JPN         | Osaka     |     155941 |
| 1667 | Otaru               | JPN         | Hokkaido  |     155784 |
| 1668 | Anjo                | JPN         | Aichi     |     153823 |
| 1669 | Narashino           | JPN         | Chiba     |     152849 |
| 1670 | Oyama               | JPN         | Tochigi   |     152820 |
| 1671 | Ogaki               | JPN         | Gifu      |     151758 |
| 1672 | Matsue              | JPN         | Shimane   |     149821 |
| 1673 | Kawanishi           | JPN         | Hyogo     |     149794 |
| 1674 | Hitachinaka         | JPN         | Tokyo-to  |     148006 |
| 1675 | Niiza               | JPN         | Saitama   |     147744 |
| 1676 | Nagareyama          | JPN         | Chiba     |     147738 |
| 1677 | Tottori             | JPN         | Tottori   |     147523 |
| 1678 | Tama                | JPN         | Ibaragi   |     146712 |
| 1679 | Iruma               | JPN         | Saitama   |     145922 |
| 1680 | Ota                 | JPN         | Gumma     |     145317 |
| 1681 | Omuta               | JPN         | Fukuoka   |     142889 |
| 1682 | Komaki              | JPN         | Aichi     |     139827 |
| 1683 | Ome                 | JPN         | Tokyo-to  |     139216 |
| 1684 | Kadoma              | JPN         | Osaka     |     138953 |
| 1685 | Yamaguchi           | JPN         | Yamaguchi |     138210 |
| 1686 | Higashimurayama     | JPN         | Tokyo-to  |     136970 |
| 1687 | Yonago              | JPN         | Tottori   |     136461 |
| 1688 | Matsubara           | JPN         | Osaka     |     135010 |
| 1689 | Musashino           | JPN         | Tokyo-to  |     134426 |
| 1690 | Tsuchiura           | JPN         | Ibaragi   |     134072 |
| 1691 | Joetsu              | JPN         | Niigata   |     133505 |
| 1692 | Miyakonojo          | JPN         | Miyazaki  |     133183 |
| 1693 | Misato              | JPN         | Saitama   |     132957 |
| 1694 | Kakamigahara        | JPN         | Gifu      |     131831 |
| 1695 | Daito               | JPN         | Osaka     |     130594 |
| 1696 | Seto                | JPN         | Aichi     |     130470 |
| 1697 | Kariya              | JPN         | Aichi     |     127969 |
| 1698 | Urayasu             | JPN         | Chiba     |     127550 |
| 1699 | Beppu               | JPN         | Oita      |     127486 |
| 1700 | Niihama             | JPN         | Ehime     |     127207 |
| 1701 | Minoo               | JPN         | Osaka     |     127026 |
| 1702 | Fujieda             | JPN         | Shizuoka  |     126897 |
| 1703 | Abiko               | JPN         | Chiba     |     126670 |
| 1704 | Nobeoka             | JPN         | Miyazaki  |     125547 |
| 1705 | Tondabayashi        | JPN         | Osaka     |     125094 |
| 1706 | Ueda                | JPN         | Nagano    |     124217 |
| 1707 | Kashihara           | JPN         | Nara      |     124013 |
| 1708 | Matsusaka           | JPN         | Mie       |     123582 |
| 1709 | Isesaki             | JPN         | Gumma     |     123285 |
| 1710 | Zama                | JPN         | Kanagawa  |     122046 |
| 1711 | Kisarazu            | JPN         | Chiba     |     121967 |
| 1712 | Noda                | JPN         | Chiba     |     121030 |
| 1713 | Ishinomaki          | JPN         | Miyagi    |     120963 |
| 1714 | Fujinomiya          | JPN         | Shizuoka  |     119714 |
| 1715 | Kawachinagano       | JPN         | Osaka     |     119666 |
| 1716 | Imabari             | JPN         | Ehime     |     119357 |
| 1717 | Aizuwakamatsu       | JPN         | Fukushima |     119287 |
| 1718 | Higashihiroshima    | JPN         | Hiroshima |     119166 |
| 1719 | Habikino            | JPN         | Osaka     |     118968 |
| 1720 | Ebetsu              | JPN         | Hokkaido  |     118805 |
| 1721 | Hofu                | JPN         | Yamaguchi |     118751 |
| 1722 | Kiryu               | JPN         | Gumma     |     118326 |
| 1723 | Okinawa             | JPN         | Okinawa   |     117748 |
| 1724 | Yaizu               | JPN         | Shizuoka  |     117258 |
| 1725 | Toyokawa            | JPN         | Aichi     |     115781 |
| 1726 | Ebina               | JPN         | Kanagawa  |     115571 |
| 1727 | Asaka               | JPN         | Saitama   |     114815 |
| 1728 | Higashikurume       | JPN         | Tokyo-to  |     111666 |
| 1729 | Ikoma               | JPN         | Nara      |     111645 |
| 1730 | Kitami              | JPN         | Hokkaido  |     111295 |
| 1731 | Koganei             | JPN         | Tokyo-to  |     110969 |
| 1732 | Iwatsuki            | JPN         | Saitama   |     110034 |
| 1733 | Mishima             | JPN         | Shizuoka  |     109699 |
| 1734 | Handa               | JPN         | Aichi     |     108600 |
| 1735 | Muroran             | JPN         | Hokkaido  |     108275 |
| 1736 | Komatsu             | JPN         | Ishikawa  |     107937 |
| 1737 | Yatsushiro          | JPN         | Kumamoto  |     107661 |
| 1738 | Iida                | JPN         | Nagano    |     107583 |
| 1739 | Tokuyama            | JPN         | Yamaguchi |     107078 |
| 1740 | Kokubunji           | JPN         | Tokyo-to  |     106996 |
| 1741 | Akishima            | JPN         | Tokyo-to  |     106914 |
| 1742 | Iwakuni             | JPN         | Yamaguchi |     106647 |
| 1743 | Kusatsu             | JPN         | Shiga     |     106232 |
| 1744 | Kuwana              | JPN         | Mie       |     106121 |
| 1745 | Sanda               | JPN         | Hyogo     |     105643 |
| 1746 | Hikone              | JPN         | Shiga     |     105508 |
| 1747 | Toda                | JPN         | Saitama   |     103969 |
| 1748 | Tajimi              | JPN         | Gifu      |     103171 |
| 1749 | Ikeda               | JPN         | Osaka     |     102710 |
| 1750 | Fukaya              | JPN         | Saitama   |     102156 |
| 1751 | Ise                 | JPN         | Mie       |     101732 |
| 1752 | Sakata              | JPN         | Yamagata  |     101651 |
| 1753 | Kasuga              | JPN         | Fukuoka   |     101344 |
| 1754 | Kamagaya            | JPN         | Chiba     |     100821 |
| 1755 | Tsuruoka            | JPN         | Yamagata  |     100713 |
| 1756 | Hoya                | JPN         | Tokyo-to  |     100313 |
| 1757 | Nishio              | JPN         | Chiba     |     100032 |
| 1758 | Tokai               | JPN         | Aichi     |      99738 |
| 1759 | Inazawa             | JPN         | Aichi     |      98746 |
| 1760 | Sakado              | JPN         | Saitama   |      98221 |
| 1761 | Isehara             | JPN         | Kanagawa  |      98123 |
| 1762 | Takasago            | JPN         | Hyogo     |      97632 |
| 1763 | Fujimi              | JPN         | Saitama   |      96972 |
| 1764 | Urasoe              | JPN         | Okinawa   |      96002 |
| 1765 | Yonezawa            | JPN         | Yamagata  |      95592 |
| 1766 | Konan               | JPN         | Aichi     |      95521 |
| 1767 | Yamatokoriyama      | JPN         | Nara      |      95165 |
| 1768 | Maizuru             | JPN         | Kyoto     |      94784 |
| 1769 | Onomichi            | JPN         | Hiroshima |      93756 |
| 1770 | Higashimatsuyama    | JPN         | Saitama   |      93342 |
| 1771 | Kimitsu             | JPN         | Chiba     |      93216 |
| 1772 | Isahaya             | JPN         | Nagasaki  |      93058 |
| 1773 | Kanuma              | JPN         | Tochigi   |      93053 |
| 1774 | Izumisano           | JPN         | Osaka     |      92583 |
| 1775 | Kameoka             | JPN         | Kyoto     |      92398 |
| 1776 | Mobara              | JPN         | Chiba     |      91664 |
| 1777 | Narita              | JPN         | Chiba     |      91470 |
| 1778 | Kashiwazaki         | JPN         | Niigata   |      91229 |
| 1779 | Tsuyama             | JPN         | Okayama   |      91170 |
+------+---------------------+-------------+-----------+------------+
248 rows in set (0.03 sec)

mysql> select * from city where CountryCode ='JPN'
    -> order by Population ASC;
+------+---------------------+-------------+-----------+------------+
| ID   | Name                | CountryCode | District  | Population |
+------+---------------------+-------------+-----------+------------+
| 1779 | Tsuyama             | JPN         | Okayama   |      91170 |
| 1778 | Kashiwazaki         | JPN         | Niigata   |      91229 |
| 1777 | Narita              | JPN         | Chiba     |      91470 |
| 1776 | Mobara              | JPN         | Chiba     |      91664 |
| 1775 | Kameoka             | JPN         | Kyoto     |      92398 |
| 1774 | Izumisano           | JPN         | Osaka     |      92583 |
| 1773 | Kanuma              | JPN         | Tochigi   |      93053 |
| 1772 | Isahaya             | JPN         | Nagasaki  |      93058 |
| 1771 | Kimitsu             | JPN         | Chiba     |      93216 |
| 1770 | Higashimatsuyama    | JPN         | Saitama   |      93342 |
| 1769 | Onomichi            | JPN         | Hiroshima |      93756 |
| 1768 | Maizuru             | JPN         | Kyoto     |      94784 |
| 1767 | Yamatokoriyama      | JPN         | Nara      |      95165 |
| 1766 | Konan               | JPN         | Aichi     |      95521 |
| 1765 | Yonezawa            | JPN         | Yamagata  |      95592 |
| 1764 | Urasoe              | JPN         | Okinawa   |      96002 |
| 1763 | Fujimi              | JPN         | Saitama   |      96972 |
| 1762 | Takasago            | JPN         | Hyogo     |      97632 |
| 1761 | Isehara             | JPN         | Kanagawa  |      98123 |
| 1760 | Sakado              | JPN         | Saitama   |      98221 |
| 1759 | Inazawa             | JPN         | Aichi     |      98746 |
| 1758 | Tokai               | JPN         | Aichi     |      99738 |
| 1757 | Nishio              | JPN         | Chiba     |     100032 |
| 1756 | Hoya                | JPN         | Tokyo-to  |     100313 |
| 1755 | Tsuruoka            | JPN         | Yamagata  |     100713 |
| 1754 | Kamagaya            | JPN         | Chiba     |     100821 |
| 1753 | Kasuga              | JPN         | Fukuoka   |     101344 |
| 1752 | Sakata              | JPN         | Yamagata  |     101651 |
| 1751 | Ise                 | JPN         | Mie       |     101732 |
| 1750 | Fukaya              | JPN         | Saitama   |     102156 |
| 1749 | Ikeda               | JPN         | Osaka     |     102710 |
| 1748 | Tajimi              | JPN         | Gifu      |     103171 |
| 1747 | Toda                | JPN         | Saitama   |     103969 |
| 1746 | Hikone              | JPN         | Shiga     |     105508 |
| 1745 | Sanda               | JPN         | Hyogo     |     105643 |
| 1744 | Kuwana              | JPN         | Mie       |     106121 |
| 1743 | Kusatsu             | JPN         | Shiga     |     106232 |
| 1742 | Iwakuni             | JPN         | Yamaguchi |     106647 |
| 1741 | Akishima            | JPN         | Tokyo-to  |     106914 |
| 1740 | Kokubunji           | JPN         | Tokyo-to  |     106996 |
| 1739 | Tokuyama            | JPN         | Yamaguchi |     107078 |
| 1738 | Iida                | JPN         | Nagano    |     107583 |
| 1737 | Yatsushiro          | JPN         | Kumamoto  |     107661 |
| 1736 | Komatsu             | JPN         | Ishikawa  |     107937 |
| 1735 | Muroran             | JPN         | Hokkaido  |     108275 |
| 1734 | Handa               | JPN         | Aichi     |     108600 |
| 1733 | Mishima             | JPN         | Shizuoka  |     109699 |
| 1732 | Iwatsuki            | JPN         | Saitama   |     110034 |
| 1731 | Koganei             | JPN         | Tokyo-to  |     110969 |
| 1730 | Kitami              | JPN         | Hokkaido  |     111295 |
| 1729 | Ikoma               | JPN         | Nara      |     111645 |
| 1728 | Higashikurume       | JPN         | Tokyo-to  |     111666 |
| 1727 | Asaka               | JPN         | Saitama   |     114815 |
| 1726 | Ebina               | JPN         | Kanagawa  |     115571 |
| 1725 | Toyokawa            | JPN         | Aichi     |     115781 |
| 1724 | Yaizu               | JPN         | Shizuoka  |     117258 |
| 1723 | Okinawa             | JPN         | Okinawa   |     117748 |
| 1722 | Kiryu               | JPN         | Gumma     |     118326 |
| 1721 | Hofu                | JPN         | Yamaguchi |     118751 |
| 1720 | Ebetsu              | JPN         | Hokkaido  |     118805 |
| 1719 | Habikino            | JPN         | Osaka     |     118968 |
| 1718 | Higashihiroshima    | JPN         | Hiroshima |     119166 |
| 1717 | Aizuwakamatsu       | JPN         | Fukushima |     119287 |
| 1716 | Imabari             | JPN         | Ehime     |     119357 |
| 1715 | Kawachinagano       | JPN         | Osaka     |     119666 |
| 1714 | Fujinomiya          | JPN         | Shizuoka  |     119714 |
| 1713 | Ishinomaki          | JPN         | Miyagi    |     120963 |
| 1712 | Noda                | JPN         | Chiba     |     121030 |
| 1711 | Kisarazu            | JPN         | Chiba     |     121967 |
| 1710 | Zama                | JPN         | Kanagawa  |     122046 |
| 1709 | Isesaki             | JPN         | Gumma     |     123285 |
| 1708 | Matsusaka           | JPN         | Mie       |     123582 |
| 1707 | Kashihara           | JPN         | Nara      |     124013 |
| 1706 | Ueda                | JPN         | Nagano    |     124217 |
| 1705 | Tondabayashi        | JPN         | Osaka     |     125094 |
| 1704 | Nobeoka             | JPN         | Miyazaki  |     125547 |
| 1703 | Abiko               | JPN         | Chiba     |     126670 |
| 1702 | Fujieda             | JPN         | Shizuoka  |     126897 |
| 1701 | Minoo               | JPN         | Osaka     |     127026 |
| 1700 | Niihama             | JPN         | Ehime     |     127207 |
| 1699 | Beppu               | JPN         | Oita      |     127486 |
| 1698 | Urayasu             | JPN         | Chiba     |     127550 |
| 1697 | Kariya              | JPN         | Aichi     |     127969 |
| 1696 | Seto                | JPN         | Aichi     |     130470 |
| 1695 | Daito               | JPN         | Osaka     |     130594 |
| 1694 | Kakamigahara        | JPN         | Gifu      |     131831 |
| 1693 | Misato              | JPN         | Saitama   |     132957 |
| 1692 | Miyakonojo          | JPN         | Miyazaki  |     133183 |
| 1691 | Joetsu              | JPN         | Niigata   |     133505 |
| 1690 | Tsuchiura           | JPN         | Ibaragi   |     134072 |
| 1689 | Musashino           | JPN         | Tokyo-to  |     134426 |
| 1688 | Matsubara           | JPN         | Osaka     |     135010 |
| 1687 | Yonago              | JPN         | Tottori   |     136461 |
| 1686 | Higashimurayama     | JPN         | Tokyo-to  |     136970 |
| 1685 | Yamaguchi           | JPN         | Yamaguchi |     138210 |
| 1684 | Kadoma              | JPN         | Osaka     |     138953 |
| 1683 | Ome                 | JPN         | Tokyo-to  |     139216 |
| 1682 | Komaki              | JPN         | Aichi     |     139827 |
| 1681 | Omuta               | JPN         | Fukuoka   |     142889 |
| 1680 | Ota                 | JPN         | Gumma     |     145317 |
| 1679 | Iruma               | JPN         | Saitama   |     145922 |
| 1678 | Tama                | JPN         | Ibaragi   |     146712 |
| 1677 | Tottori             | JPN         | Tottori   |     147523 |
| 1676 | Nagareyama          | JPN         | Chiba     |     147738 |
| 1675 | Niiza               | JPN         | Saitama   |     147744 |
| 1674 | Hitachinaka         | JPN         | Tokyo-to  |     148006 |
| 1673 | Kawanishi           | JPN         | Hyogo     |     149794 |
| 1672 | Matsue              | JPN         | Shimane   |     149821 |
| 1671 | Ogaki               | JPN         | Gifu      |     151758 |
| 1670 | Oyama               | JPN         | Tochigi   |     152820 |
| 1669 | Narashino           | JPN         | Chiba     |     152849 |
| 1668 | Anjo                | JPN         | Aichi     |     153823 |
| 1667 | Otaru               | JPN         | Hokkaido  |     155784 |
| 1666 | Moriguchi           | JPN         | Osaka     |     155941 |
| 1665 | Kumagaya            | JPN         | Saitama   |     157171 |
| 1664 | Tachikawa           | JPN         | Tokyo-to  |     159430 |
| 1663 | Tsukuba             | JPN         | Ibaragi   |     160768 |
| 1662 | Yachiyo             | JPN         | Chiba     |     161222 |
| 1661 | Sayama              | JPN         | Saitama   |     162472 |
| 1660 | Tsu                 | JPN         | Mie       |     164543 |
| 1659 | Ashikaga            | JPN         | Tochigi   |     165243 |
| 1658 | Hadano              | JPN         | Kanagawa  |     166512 |
| 1657 | Hino                | JPN         | Tokyo-to  |     166770 |
| 1656 | Izumi               | JPN         | Osaka     |     166979 |
| 1655 | Mitaka              | JPN         | Tokyo-to  |     167268 |
| 1654 | Kamakura            | JPN         | Kanagawa  |     167661 |
| 1653 | Sakura              | JPN         | Chiba     |     168072 |
| 1652 | Saga                | JPN         | Saga      |     170034 |
| 1651 | Tomakomai           | JPN         | Hokkaido  |     171958 |
| 1650 | Obihiro             | JPN         | Hokkaido  |     173685 |
| 1649 | Takaoka             | JPN         | Toyama    |     174380 |
| 1648 | Kodaira             | JPN         | Tokyo-to  |     174984 |
| 1647 | Ube                 | JPN         | Yamaguchi |     175206 |
| 1646 | Hirosaki            | JPN         | Aomori    |     177522 |
| 1645 | Suzuka              | JPN         | Mie       |     184061 |
| 1644 | Uji                 | JPN         | Kyoto     |     188735 |
| 1643 | Itami               | JPN         | Hyogo     |     190886 |
| 1642 | Nagaoka             | JPN         | Niigata   |     192407 |
| 1641 | Hitachi             | JPN         | Ibaragi   |     196622 |
| 1640 | Kishiwada           | JPN         | Osaka     |     197276 |
| 1639 | Kushiro             | JPN         | Hokkaido  |     197608 |
| 1638 | Kofu                | JPN         | Yamanashi |     199753 |
| 1637 | Odawara             | JPN         | Kanagawa  |     200171 |
| 1636 | Chofu               | JPN         | Tokyo-to  |     201585 |
| 1635 | Kasukabe            | JPN         | Saitama   |     201838 |
| 1634 | Takarazuka          | JPN         | Hyogo     |     205993 |
| 1633 | Kure                | JPN         | Hiroshima |     206504 |
| 1632 | Matsumoto           | JPN         | Nagano    |     206801 |
| 1631 | Yamato              | JPN         | Kanagawa  |     208234 |
| 1630 | Ageo                | JPN         | Saitama   |     209442 |
| 1629 | Numazu              | JPN         | Shizuoka  |     211382 |
| 1628 | Atsugi              | JPN         | Kanagawa  |     212407 |
| 1627 | Chigasaki           | JPN         | Kanagawa  |     216015 |
| 1626 | Fuchu               | JPN         | Tokyo-to  |     220576 |
| 1625 | Soka                | JPN         | Saitama   |     222768 |
| 1624 | Fuji                | JPN         | Shizuoka  |     231527 |
| 1623 | Kurume              | JPN         | Fukuoka   |     235611 |
| 1622 | Shimizu             | JPN         | Shizuoka  |     239123 |
| 1621 | Takasaki            | JPN         | Gumma     |     239124 |
| 1620 | Hachinohe           | JPN         | Aomori    |     242979 |
| 1619 | Sasebo              | JPN         | Nagasaki  |     244240 |
| 1618 | Mito                | JPN         | Ibaragi   |     246559 |
| 1617 | Hiratsuka           | JPN         | Kanagawa  |     254207 |
| 1616 | Fukui               | JPN         | Fukui     |     254818 |
| 1615 | Yamagata            | JPN         | Yamagata  |     255617 |
| 1614 | Shimonoseki         | JPN         | Yamaguchi |     257263 |
| 1613 | Neyagawa            | JPN         | Osaka     |     257315 |
| 1612 | Ibaraki             | JPN         | Osaka     |     261020 |
| 1611 | Kakogawa            | JPN         | Hyogo     |     266281 |
| 1610 | Tokushima           | JPN         | Tokushima |     269649 |
| 1609 | Ichinomiya          | JPN         | Aichi     |     270828 |
| 1608 | Yao                 | JPN         | Osaka     |     276421 |
| 1607 | Ichihara            | JPN         | Chiba     |     279280 |
| 1606 | Otsu                | JPN         | Shiga     |     282070 |
| 1605 | Kasugai             | JPN         | Aichi     |     282348 |
| 1604 | Maebashi            | JPN         | Gumma     |     284473 |
| 1603 | Morioka             | JPN         | Iwate     |     287353 |
| 1602 | Fukushima           | JPN         | Fukushima |     287525 |
| 1601 | Yokkaichi           | JPN         | Mie       |     288173 |
| 1600 | Akashi              | JPN         | Hyogo     |     292253 |
| 1599 | Hakodate            | JPN         | Hokkaido  |     294788 |
| 1598 | Aomori              | JPN         | Aomori    |     295969 |
| 1597 | Naha                | JPN         | Okinawa   |     299851 |
| 1596 | Koshigaya           | JPN         | Saitama   |     301446 |
| 1595 | Miyazaki            | JPN         | Miyazaki  |     303784 |
| 1594 | Akita               | JPN         | Akita     |     314440 |
| 1593 | Kashiwa             | JPN         | Chiba     |     320296 |
| 1592 | Kochi               | JPN         | Kochi     |     324710 |
| 1591 | Toyama              | JPN         | Toyama    |     325790 |
| 1590 | Tokorozawa          | JPN         | Saitama   |     325809 |
| 1589 | Kawagoe             | JPN         | Saitama   |     327211 |
| 1588 | Okazaki             | JPN         | Aichi     |     328711 |
| 1587 | Koriyama            | JPN         | Fukushima |     330335 |
| 1586 | Takamatsu           | JPN         | Kagawa    |     332471 |
| 1585 | Suita               | JPN         | Osaka     |     345750 |
| 1584 | Toyota              | JPN         | Aichi     |     346090 |
| 1583 | Toyohashi           | JPN         | Aichi     |     360066 |
| 1582 | Nagano              | JPN         | Nagano    |     361391 |
| 1581 | Iwaki               | JPN         | Fukushima |     361737 |
| 1580 | Takatsuki           | JPN         | Osaka     |     361747 |
| 1579 | Nara                | JPN         | Nara      |     362812 |
| 1578 | Machida             | JPN         | Tokyo-to  |     364197 |
| 1577 | Asahikawa           | JPN         | Hokkaido  |     364813 |
| 1576 | Fujisawa            | JPN         | Kanagawa  |     372840 |
| 1575 | Fukuyama            | JPN         | Hiroshima |     376921 |
| 1574 | Wakayama            | JPN         | Wakayama  |     391233 |
| 1573 | Toyonaka            | JPN         | Osaka     |     396689 |
| 1572 | Nishinomiya         | JPN         | Hyogo     |     397618 |
| 1571 | Hirakata            | JPN         | Osaka     |     403151 |
| 1570 | Gifu                | JPN         | Gifu      |     408007 |
| 1569 | Kurashiki           | JPN         | Okayama   |     425103 |
| 1568 | Yokosuka            | JPN         | Kanagawa  |     430200 |
| 1567 | Nagasaki            | JPN         | Nagasaki  |     432759 |
| 1566 | Oita                | JPN         | Oita      |     433401 |
| 1565 | Utsunomiya          | JPN         | Tochigi   |     440353 |
| 1564 | Omiya               | JPN         | Saitama   |     441649 |
| 1563 | Ichikawa            | JPN         | Chiba     |     441893 |
| 1562 | Kawaguchi           | JPN         | Saitama   |     452155 |
| 1561 | Kanazawa            | JPN         | Ishikawa  |     455386 |
| 1560 | Matsudo             | JPN         | Chiba     |     461126 |
| 1559 | Matsuyama           | JPN         | Ehime     |     466133 |
| 1558 | Urawa               | JPN         | Saitama   |     469675 |
| 1557 | Shizuoka            | JPN         | Shizuoka  |     473854 |
| 1556 | Himeji              | JPN         | Hyogo     |     475167 |
| 1555 | Amagasaki           | JPN         | Hyogo     |     481434 |
| 1554 | Niigata             | JPN         | Niigata   |     497464 |
| 1553 | Hachioji            | JPN         | Tokyo-to  |     513451 |
| 1552 | Higashiosaka        | JPN         | Osaka     |     517785 |
| 1551 | Funabashi           | JPN         | Chiba     |     545299 |
| 1550 | Kagoshima           | JPN         | Kagoshima |     549977 |
| 1549 | Hamamatsu           | JPN         | Shizuoka  |     568796 |
| 1548 | Sagamihara          | JPN         | Kanagawa  |     586300 |
| 1547 | Okayama             | JPN         | Okayama   |     624269 |
| 1546 | Kumamoto            | JPN         | Kumamoto  |     656734 |
| 1545 | Sakai               | JPN         | Osaka     |     797735 |
| 1544 | Chiba               | JPN         | Chiba     |     863930 |
| 1543 | Sendai              | JPN         | Miyagi    |     989975 |
| 1542 | Kitakyushu          | JPN         | Fukuoka   |    1016264 |
| 1541 | Hiroshima           | JPN         | Hiroshima |    1119117 |
| 1540 | Kawasaki            | JPN         | Kanagawa  |    1217359 |
| 1539 | Fukuoka             | JPN         | Fukuoka   |    1308379 |
| 1538 | Kobe                | JPN         | Hyogo     |    1425139 |
| 1537 | Kioto               | JPN         | Kyoto     |    1461974 |
| 1536 | Sapporo             | JPN         | Hokkaido  |    1790886 |
| 1535 | Nagoya              | JPN         | Aichi     |    2154376 |
| 1534 | Osaka               | JPN         | Osaka     |    2595674 |
| 1533 | Jokohama [Yokohama] | JPN         | Kanagawa  |    3339594 |
| 1532 | Tokyo               | JPN         | Tokyo-to  |    7980230 |
+------+---------------------+-------------+-----------+------------+
248 rows in set (0.01 sec)


mysql> select Name from city where CountryCode IN ('CZE','PRI','EST');
+------------------+
| Name             |
+------------------+
| Praha            |
| Brno             |
| Ostrava          |
| Plzen            |
| Olomouc          |
| Liberec          |
| Ceské Budejovice |
| Hradec Králové   |
| Ústí nad Labem   |
| Pardubice        |
| Tallinn          |
| Tartu            |
| San Juan         |
| Bayamón          |
| Ponce            |
| Carolina         |
| Caguas           |
| Arecibo          |
| Guaynabo         |
| Mayagüez         |
| Toa Baja         |
+------------------+
21 rows in set (0.00 sec)

```
