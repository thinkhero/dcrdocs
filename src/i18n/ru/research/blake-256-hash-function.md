# Хеш-функция BLAKE-256 

---

SHA256, используемый в Bitcoin, имеет ряд технических недостатков из-за своей структуры Меркла-Дамгарда. Эти уязвимости привели к конкуренции SHA3 за новую хеш-функцию, основанную на другой фундаментальной структуре. Decred выбрал для себя хеш-функцию BLAKE256, как финалиста данного соревнования[^1] [^2]. Данная хеш-функция основана на конструкции HAIFA, которая включает в себя вариацию шифрования потока ChaCha от Bernstein. Хеш-функция отличается высокой производительностью на микроархитектуре x86-64, будучи более быстрой для коротких сообщений, чем SHA256[^3] несмотря на то, что считается, что она имеет гораздо более высокий запас прочности на 14-rounds.

---

## <i class="fa fa-book"></i> Ссылки 

[^1]: Aumasson J., Henzen L., Meier W., Phan R. 2010. [SHA-3 proposal BLAKE](https://decred.org/research/aumasson2010.pdf).
[^2]: Aumasson J., Henzen L., Meier W., Phan R. 2014. The hash function BLAKE.
[^3]: Bernstein D. and Lange T. 2013. [eBACS: ECRYPT benchmarking of cryptographic systems](http://bench.cr.yp.to).