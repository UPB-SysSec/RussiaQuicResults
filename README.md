# On Russia’s Early Introduction of QUIC SNI Censorship

This repository contains pcaps, results, and archived references for the FOCI submission "On Russia’s Early Introduction of QUIC SNI Censorship".

- `archived-posts`:
  Archived forum posts referenced in the paper.
- `parsing`:
  QUIC parsing payloads and results.
- `ports`:
  Pcaps from the port scans.
- `ttl`:
  Pcaps from TTL measurements.
- `domains`:
  Condensed results from the domain scans at our vantage points in Moscow and Saint Petersburg.


We anonymized the recorded pcaps using the following IP address mapping:

| Abbr. | Location         | IP address   |
|-------|------------------|--------------|
| MOW   | Moscow           | 10.0.0.1     |
| SPE   | Saint Petersburg | 10.0.0.2     |
| NVS   | Novosibirsk      | 10.0.0.3     |
|       | Uncensored       | 10.0.255.255 |


## Archived Forum Posts

The directory `archived-posts` contains forum threads discussing QUIC censorship in Russia. We provide the archived forum posts as PDF and text files.

**Note:** The urls on the forum `ntc.party` follow the format `https://ntc.party/t/<thread id>/<post id>`. The archived files are named according to the thread ID. You can find the number of each post next to the post's username.

Referenced posts:
- [4] anonymous28. 2022. Forum Post: “Система может расшифровать QUIC_V1 и декодировать SNI.”. https://ntc.party/t/1823/32 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [5] anonymous57. 2022. Forum Post: “Локалхост в надежных руках. [...]”. https://ntc.party/t/1823/69 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [11] bolvan. 2022. Forum Post: “Подтверждаю. Добавлю к этому, что к входящим пакетам фильтрация не применяется и используется stateful фильтр[...]”. https://ntc.party/t/1823/11 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [12] bolvan. 2023. Forum Post: “Текущая ситуация по QUIC примерно такая. [...]”. https://ntc.party/t/1823/74 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [23] loskiq. 2024. Forum Post: “видимо, начали блочить домен www.youtube.com по SNI [...]”. https://ntc.party/t/8055/145 [(PDF)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.txt)
- [25] Molchun. 2025. Forum Post: “В то время как на йоте полный блок ВСЕХ ресурсов. [...]”. https://ntc.party/t/8055/337 [(PDF)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.txt)
- [36] serfreeman1337. 2022. Forum Post: “Не устанавливается соединение по QUIC для зарубежных сайтов. [...]”. https://ntc.party/t/1823/1 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [40] ValdikSS. 2022. Forum Post: “Фильтр работает только для пакетов с UDPнагрузкой больше 1001 байтов (включительно). [...]”. https://ntc.party/t/1823/10 [(PDF)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/1823%20-%20Ограничение%20HTTP_3%20(QUIC)%20-%20Russia%20-%20NTC.txt)
- [41] ValdikSS. 2024. Forum Post: “Замедляют по SNI *.googlevideo.com — домена, с которого раздаётся видео YouTube,”. https://ntc.party/t/8055/2 [(PDF)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.txt)
- [42] ValdikSS. 2024. Forum Post: “Начали замедлять и QUIC (HTTP/3) тоже. [...]”. https://ntc.party/t/8055/79 [(PDF)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.pdf) [(TXT)](archived-posts/8055%20-%20Замедление_блокировка%20YouTube%20в%20России%20-%20Russia%20-%20NTC.txt)
