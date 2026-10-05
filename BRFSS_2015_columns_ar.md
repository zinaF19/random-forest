# أعمدة BRFSS 2015 باختصار

- الأعمدة التي تبدأ بـ `_` **محسوبة** (Calculated).
- **1** = نعم، **2** = لا · **7/77** = لا يعرف · **9/99** = رفض ← حوّليها إلى `NaN` · **88** = صفر أيام.

## 1. الهدف (Target)
- `label`: الصحة العامة (1 = جيدة، 2 = سيئة)، غالبًا هو `_RFHLTH`

## 2. الديموغرافيا (Demographics)
- `SEX` الجنس · `MARITAL` الحالة الاجتماعية · `EDUCA` `_EDUCAG` التعليم · `EMPLOY1` العمل · `INCOME2` `_INCOMG` الدخل
- `RENTHOM1` ملك/إيجار · `VETERAN3` محارب قديم · `CHILDREN` `_CHLDCNT` عدد الأطفال · `INTERNET` الإنترنت · `PREGNANT` حامل
- العمر (Age): `_AGEG5YR` `_AGE65YR` `_AGE80` `_AGE_G`
- العِرق (Race): `_RACE` `_RACEG21` `_RACEGR3` `_RACE_G1` `_PRACE1` `_MRACE1` `_HISPANC`

## 3. الجسم (Body / BMI)
- `WEIGHT2` `HEIGHT3` الوزن والطول (خام) · `WTKG3` الوزن كغ×100 · `HTIN4` `HTM4` الطول بالإنش/سم
- `_BMI5` مؤشر كتلة الجسم ×100 · `_BMI5CAT` فئته · `_RFBMI5` زيادة وزن/سمنة

## 4. الرعاية الصحية (Health Care)
- `PERSDOC2` طبيب شخصي · `MEDCOST` لم يزر الطبيب بسبب التكلفة · `CHECKUP1` آخر فحص · `_HCVU651` تأمين صحي

## 5. الضغط والكوليسترول
- `BPHIGH4` `_RFHYPE5` ضغط مرتفع · `BPMEDS` دواء الضغط
- `BLOODCHO` `CHOLCHK` `_CHOLCHK` فحص الكوليسترول · `TOLDHI2` `_RFCHOL` كوليسترول مرتفع

## 6. الأمراض المزمنة (Chronic Diseases)
- `CVDINFR4` نوبة قلبية · `CVDCRHD4` مرض تاجي · `_MICHD` أحدهما · `CVDSTRK3` سكتة دماغية
- `ASTHMA3` `ASTHNOW` `_LTASTH1` `_CASTHM1` `_ASTHMS1` الربو
- `CHCSCNCR` سرطان الجلد · `CHCOCNCR` سرطان آخر · `CHCCOPD1` انسداد رئوي (COPD) · `CHCKIDNY` الكلى
- `HAVARTH3` `_DRDXAR1` التهاب المفاصل · `ADDEPEV2` اكتئاب · `DIABETE3` السكري · `DIABAGE2` عمر تشخيص السكري

## 7. الإعاقة (Disability)
- `QLACTLM2` محدودية النشاط · `USEEQUIP` معدات مساعدة · `BLIND` ضعف البصر · `DECIDE` صعوبة التركيز
- `DIFFWALK` المشي · `DIFFDRES` ارتداء الملابس · `DIFFALON` الخروج وحده

## 8. التدخين (Smoking)
- `SMOKE100` دخّن 100 سيجارة · `SMOKDAY2` يدخّن حاليًا · `STOPSMK2` حاول الإقلاع · `LASTSMK2` آخر سيجارة
- `USENOW3` تبغ بدون دخان · `_SMOKER3` `_RFSMOK3` حالة التدخين

## 9. الكحول (Alcohol)
- `ALCDAY5` أيام الشرب · `AVEDRNK2` متوسط المشروبات · `DRNK3GE5` مرات الإفراط · `MAXDRNKS` أكبر عدد
- `DRNKANY5` `DROCDY3_` `_DRNKWEK` كميات محسوبة · `_RFBING5` إفراط (Binge) · `_RFDRHV5` شرب كثيف

## 10. الفواكه والخضروات (Diet)
- خام: `FRUITJU1` عصير · `FRUIT1` فواكه · `FVBEANS` بقوليات · `FVGREEN` خضار ورقية · `FVORANG` خضار برتقالية · `VEGETAB1` خضار أخرى
- يوميًا (محسوب): `FTJUDA1_` `FRUTDA1_` `BEANDAY_` `GRENDAY_` `ORNGDAY_` `VEGEDA1_`
- ملخّص: `_FRUTSUM` `_VEGESUM` المجموع · `_FRTLT1` `_VEGLT1` أقل من مرة يوميًا

## 11. النشاط البدني (Physical Activity)
- خام: `EXERANY2` أي رياضة · `EXRACT11` `EXRACT21` النوع · `EXEROFT1` `EXEROFT2` التكرار · `EXERHMM1` `EXERHMM2` المدة · `STRENGTH` تمارين القوة
- تفاصيل محسوبة: `METVL11_` `METVL21_` `MAXVO2_` `FC60_` `ACTIN11_` `ACTIN21_` `PADUR1_` `PADUR2_` `PAFREQ1_` `PAFREQ2_` `_MINAC11` `_MINAC21` `STRFREQ_` `PAMISS1_` `PAMIN11_` `PAMIN21_` `PA1MIN_` `PAVIG11_` `PAVIG21_` `PA1VIGM_`
- ملخّص (الأفضل للنموذج): `_TOTINDA` أي نشاط · `_PACAT1` فئة النشاط · `_PAINDX1` `_PA150R2` `_PA300R2` `_PA30021` `_PASTRNG` `_PAREC1` `_PASTAE1` تحقيق التوصيات

## 12. المفاصل، الحزام، اللقاحات، HIV
- المفاصل: `LMTJOIN3` `ARTHDIS2` `ARTHSOCL` `JOINPAIN` `_LMTACT1` `_LMTWRK1` `_LMTSCL1`
- حزام الأمان: `SEATBELT` `_RFSEAT2` `_RFSEAT3`
- اللقاحات: `FLUSHOT6` `FLSHTMY2` `IMFVPLAC` `_FLSHOT6` إنفلونزا · `PNEUVAC3` `_PNEUMO2` رئوي · `TETANUS` كزاز · `HPVADVC2` `HPVADSHT` HPV · `SHINGLE2` هربس نطاقي
- HIV: `HIVTST6` `HIVTSTD3` `WHRTST10` `_AIDTST3`

## 13. وحدات اختيارية (Optional Modules) ← فقد عالٍ، غالبًا تُحذف
- السكري: `PDIABTST` `PREDIAB1` `INSULIN` `BLDSUGAR` `FEETCHK2` `DOCTDIAB` `CHKHEMO3` `FEETCHK` `EYEEXAM` `DIABEYE` `DIABEDU`
- رعاية الآخرين (Caregiver): `CAREGIV1` `CRGVREL1` `CRGVLNG1` `CRGVHRS1` `CRGVPRB1` `CRGVPERS` `CRGVHOUS` `CRGVMST2` `CRGVEXPT`
- البصر: `VIDFCLT2` `VIREDIF3` `VIPRFVS2` `VINOCRE2` `VIEYEXM2` `VIINSUR2` `VICTRCT4` `VIGLUMA2` `VIMACDG2`
- الذاكرة: `CIMEMLOS` `CDHOUSE` `CDASSIST` `CDHELP` `CDSOCIAL` `CDDISCUS`
- الملح: `WTCHSALT` `LONGWTCH` `DRADVISE`
- تاريخ الربو: `ASTHMAGE` `ASATTACK` `ASERVIST` `ASDRVIST` `ASRCHKUP` `ASACTLIM` `ASYMPTOM` `ASNOSLEP` `ASTHMED3` `ASINHALR`
- القلب والأسبرين: `HAREHAB1` `STREHAB1` `CVDASPRN` `ASPUNSAF` `RLIVPAIN` `RDUCHART` `RDUCSTRK`
- إدارة المفاصل: `ARTTODAY` `ARTHWGT` `ARTHEXER` `ARTHEDU`
- فحوص السرطان: `HADMAM` `HOWLONG` `PROFEXAM` `LENGEXAM` `HADPAP2` `LASTPAP2` `HPVTEST` `HPLSTTST` `HADHYST2` `BLDSTOOL` `LSTBLDS3` `HADSIGM3` `HADSGCO1` `LASTSIG3` `PCPSAAD2` `PCPSADI1` `PCPSARE1` `PSATEST1` `PSATIME` `PCPSARS1` `PCPSADE1`
- الظروف الاجتماعية: `SCNTMNY1` `SCNTMEL1` `SCNTPAID` `SCNTWRK1` `SCNTLPAD` `SCNTLWK1`
- التوجه والهوية: `SXORIENT` `TRNSGNDR` · الدعم والرضا: `EMTSUPRT` `LSATISFY`
- الاكتئاب والقلق (PHQ-8): `ADPLEASR` `ADDOWN` `ADSLEEP` `ADENERGY` `ADEAT1` `ADFAIL` `ADTHINK` `ADMOVE` `MISTMNT` `ADANXEV`
- طفل في المنزل: `RCSGENDR` `RCSRLTN2` `CASTHDX2` `CASTHNO2` `_CHISPNC` `_CRACE1` `_CPRACE` `_CLLCPWT`

## 14. احذفيها (Drop) ← ليست ميزات
- جودة البيانات: `_MISFRTN` `_MISVEGN` `_FRTRESP` `_VEGRESP` `_FRT16` `_VEG23` `_FRUITEX` `_VEGETEX`
- المقابلة: `_STATE` `FMONTH` `DISPCODE` `SEQNO` `QSTVER` `QSTLANG` `MSCODE`
- الهاتف والمنزل: `CTELENUM` `CTELNUM1` `PVTRESD1` `PVTRESD2` `COLGHOUS` `CCLGHOUS` `STATERES` `CSTATE` `CELLFON2` `CELLFON3` `LADULT` `CADULT` `LANDLINE` `CPDEMO1` `NUMHHOL2` `NUMPHON2` `NUMADULT` `HHADULT` `NUMMEN` `NUMWOMEN`
- الأوزان (Weights): `_PSU` `_STSTR` `_STRWT` `_RAWRAKE` `_WT2RAKE` `_DUALUSE` `_DUALCOR` `_LLCPWT`
