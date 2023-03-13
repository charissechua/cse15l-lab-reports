# Lab Report 5
Charisse Chua


I decided to do what we did in lab report 3, except I am now exploring the `find` command instead of the `grep` command. 
***

These are the four commands I am testing:
1. `find ./GFG -name sample.txt`
2. `find ./GFG -empty`
3. `find . -type f -name "*.txt"`
4. `find /tmp -type f -name ".*"`


## 1. `find ./directory -name sample.txt`
Finds the file with that specific name within that specified directory. In my case, I went into the skill-demo1-data directory and searched for that specific text file and received the following output.

`find ./GFG -name something.txt` output: 

`./skill-demo1-data/something.txt`

## 2. `find ./directory -empty`
Finds the files/folders in the given directory that are empty. In my case, I searched through the skill-demo1-data library to find the empty files.

`find ./skill-demo1-data -empty` output:
```./skill-demo1-data/.git/branches
./skill-demo1-data/.git/refs/tags
./skill-demo1-data/.git/objects/info
./skill-demo1-data/written_2/demoResults.txt
```

## 3. `find . -type f -name "*.txt"`

Finds all the files that ends in the given extension. In this case, I searched through the skill-demo1-data library to find all the files that ended in `.txt` and received the following output: 

`find . -type f -name "*.txt"` output:
```./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch6.txt
./written_2/non-fiction/OUP/Abernathy/ch7.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Abernathy/ch9.txt
./written_2/non-fiction/OUP/Berk/CH4.txt
./written_2/non-fiction/OUP/Berk/ch1.txt
./written_2/non-fiction/OUP/Berk/ch2.txt
./written_2/non-fiction/OUP/Berk/ch7.txt
./written_2/non-fiction/OUP/Castro/chA.txt
./written_2/non-fiction/OUP/Castro/chB.txt
./written_2/non-fiction/OUP/Castro/chC.txt
./written_2/non-fiction/OUP/Castro/chL.txt
./written_2/non-fiction/OUP/Castro/chM.txt
./written_2/non-fiction/OUP/Castro/chN.txt
./written_2/non-fiction/OUP/Castro/chO.txt
./written_2/non-fiction/OUP/Castro/chP.txt
./written_2/non-fiction/OUP/Castro/chQ.txt
./written_2/non-fiction/OUP/Castro/chR.txt
./written_2/non-fiction/OUP/Castro/chV.txt
./written_2/non-fiction/OUP/Castro/chW.txt
./written_2/non-fiction/OUP/Castro/chY.txt
./written_2/non-fiction/OUP/Castro/chZ.txt
./written_2/non-fiction/OUP/Fletcher/ch1.txt
./written_2/non-fiction/OUP/Fletcher/ch10.txt
./written_2/non-fiction/OUP/Fletcher/ch2.txt
./written_2/non-fiction/OUP/Fletcher/ch5.txt
./written_2/non-fiction/OUP/Fletcher/ch6.txt
./written_2/non-fiction/OUP/Fletcher/ch9.txt
./written_2/non-fiction/OUP/Kauffman/ch1.txt
./written_2/non-fiction/OUP/Kauffman/ch10.txt
./written_2/non-fiction/OUP/Kauffman/ch3.txt
./written_2/non-fiction/OUP/Kauffman/ch4.txt
./written_2/non-fiction/OUP/Kauffman/ch5.txt
./written_2/non-fiction/OUP/Kauffman/ch6.txt
./written_2/non-fiction/OUP/Kauffman/ch7.txt
./written_2/non-fiction/OUP/Kauffman/ch8.txt
./written_2/non-fiction/OUP/Kauffman/ch9.txt
./written_2/non-fiction/OUP/Rybczynski/ch1.txt
./written_2/non-fiction/OUP/Rybczynski/ch2.txt
./written_2/non-fiction/OUP/Rybczynski/ch3.txt
./written_2/travel_guides/berlitz1/HandRHawaii.txt
./written_2/travel_guides/berlitz1/HandRHongKong.txt
./written_2/travel_guides/berlitz1/HandRIbiza.txt
./written_2/travel_guides/berlitz1/HandRIsrael.txt
./written_2/travel_guides/berlitz1/HandRIstanbul.txt
./written_2/travel_guides/berlitz1/HandRJamaica.txt
./written_2/travel_guides/berlitz1/HandRJerusalem.txt
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
./written_2/travel_guides/berlitz1/HandRLasVegas.txt
./written_2/travel_guides/berlitz1/HandRLisbon.txt
./written_2/travel_guides/berlitz1/HandRLosAngeles.txt
./written_2/travel_guides/berlitz1/HandRMadeira.txt
./written_2/travel_guides/berlitz1/HandRMadrid.txt
./written_2/travel_guides/berlitz1/HandRMallorca.txt
./written_2/travel_guides/berlitz1/HistoryDublin.txt
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
./written_2/travel_guides/berlitz1/HistoryEgypt.txt
./written_2/travel_guides/berlitz1/HistoryFWI.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt
./written_2/travel_guides/berlitz1/HistoryGreek.txt
./written_2/travel_guides/berlitz1/HistoryHawaii.txt
./written_2/travel_guides/berlitz1/HistoryHongKong.txt
./written_2/travel_guides/berlitz1/HistoryIbiza.txt
./written_2/travel_guides/berlitz1/HistoryIndia.txt
./written_2/travel_guides/berlitz1/HistoryIsrael.txt
./written_2/travel_guides/berlitz1/HistoryIstanbul.txt
./written_2/travel_guides/berlitz1/HistoryItaly.txt
./written_2/travel_guides/berlitz1/HistoryJamaica.txt
./written_2/travel_guides/berlitz1/HistoryJapan.txt
./written_2/travel_guides/berlitz1/HistoryJerusalem.txt
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
./written_2/travel_guides/berlitz1/HistoryLasVegas.txt
./written_2/travel_guides/berlitz1/HistoryMadeira.txt
./written_2/travel_guides/berlitz1/HistoryMadrid.txt
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt
./written_2/travel_guides/berlitz1/HistoryMallorca.txt
./written_2/travel_guides/berlitz1/IntroDublin.txt
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt
./written_2/travel_guides/berlitz1/IntroEgypt.txt
./written_2/travel_guides/berlitz1/IntroFWI.txt
./written_2/travel_guides/berlitz1/IntroFrance.txt
./written_2/travel_guides/berlitz1/IntroGreek.txt
./written_2/travel_guides/berlitz1/IntroHongKong.txt
./written_2/travel_guides/berlitz1/IntroIbiza.txt
./written_2/travel_guides/berlitz1/IntroIndia.txt
./written_2/travel_guides/berlitz1/IntroIsrael.txt
./written_2/travel_guides/berlitz1/IntroIstanbul.txt
./written_2/travel_guides/berlitz1/IntroItaly.txt
./written_2/travel_guides/berlitz1/IntroJamaica.txt
./written_2/travel_guides/berlitz1/IntroJapan.txt
./written_2/travel_guides/berlitz1/IntroJerusalem.txt
./written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
./written_2/travel_guides/berlitz1/IntroLasVegas.txt
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt
./written_2/travel_guides/berlitz1/IntroMadeira.txt
./written_2/travel_guides/berlitz1/IntroMadrid.txt
./written_2/travel_guides/berlitz1/IntroMalaysia.txt
./written_2/travel_guides/berlitz1/IntroMallorca.txt
./written_2/travel_guides/berlitz1/JungleMalaysia.txt
./written_2/travel_guides/berlitz1/WhatToDublin.txt
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
./written_2/travel_guides/berlitz1/WhatToEgypt.txt
./written_2/travel_guides/berlitz1/WhatToFWI.txt
./written_2/travel_guides/berlitz1/WhatToFrance.txt
./written_2/travel_guides/berlitz1/WhatToGreek.txt
./written_2/travel_guides/berlitz1/WhatToHawaii.txt
./written_2/travel_guides/berlitz1/WhatToHongKong.txt
./written_2/travel_guides/berlitz1/WhatToIbiza.txt
./written_2/travel_guides/berlitz1/WhatToIndia.txt
./written_2/travel_guides/berlitz1/WhatToIsrael.txt
./written_2/travel_guides/berlitz1/WhatToIstanbul.txt
./written_2/travel_guides/berlitz1/WhatToItaly.txt
./written_2/travel_guides/berlitz1/WhatToJamaica.txt
./written_2/travel_guides/berlitz1/WhatToJapan.txt
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
./written_2/travel_guides/berlitz1/WhatToMadeira.txt
./written_2/travel_guides/berlitz1/WhatToMalaysia.txt
./written_2/travel_guides/berlitz1/WhatToMallorca.txt
./written_2/travel_guides/berlitz1/WhereToDublin.txt
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
./written_2/travel_guides/berlitz1/WhereToEgypt.txt
./written_2/travel_guides/berlitz1/WhereToFWI.txt
./written_2/travel_guides/berlitz1/WhereToFrance.txt
./written_2/travel_guides/berlitz1/WhereToGreek.txt
./written_2/travel_guides/berlitz1/WhereToHawaii.txt
./written_2/travel_guides/berlitz1/WhereToHongKong.txt
./written_2/travel_guides/berlitz1/WhereToIbiza.txt
./written_2/travel_guides/berlitz1/WhereToIndia.txt
./written_2/travel_guides/berlitz1/WhereToIsrael.txt
./written_2/travel_guides/berlitz1/WhereToIstanbul.txt
./written_2/travel_guides/berlitz1/WhereToItaly.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt
./written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
./written_2/travel_guides/berlitz1/WhereToMadeira.txt
./written_2/travel_guides/berlitz1/WhereToMadrid.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
./written_2/travel_guides/berlitz1/WhereToMallorca.txt
./written_2/travel_guides/berlitz2/Algarve-History.txt
./written_2/travel_guides/berlitz2/Algarve-Intro.txt
./written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
./written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
./written_2/travel_guides/berlitz2/Amsterdam-History.txt
./written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
./written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
./written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
./written_2/travel_guides/berlitz2/Athens-History.txt
./written_2/travel_guides/berlitz2/Athens-Intro.txt
./written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
./written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
./written_2/travel_guides/berlitz2/Bahamas-History.txt
./written_2/travel_guides/berlitz2/Bahamas-Intro.txt
./written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
./written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
./written_2/travel_guides/berlitz2/Bali-History.txt
./written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
./written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
./written_2/travel_guides/berlitz2/Barcelona-History.txt
./written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
./written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
./written_2/travel_guides/berlitz2/Beijing-History.txt
./written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
./written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
./written_2/travel_guides/berlitz2/Berlin-History.txt
./written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
./written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
./written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
./written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
./written_2/travel_guides/berlitz2/Bermuda-history.txt
./written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
./written_2/travel_guides/berlitz2/Budapest-History.txt
./written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
./written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
./written_2/travel_guides/berlitz2/California-History.txt
./written_2/travel_guides/berlitz2/California-WhatToDo.txt
./written_2/travel_guides/berlitz2/California-WhereToGo.txt
./written_2/travel_guides/berlitz2/Canada-History.txt
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
./written_2/travel_guides/berlitz2/CanaryIslands-History.txt
./written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
./written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
./written_2/travel_guides/berlitz2/Cancun-History.txt
./written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
./written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
./written_2/travel_guides/berlitz2/China-History.txt
./written_2/travel_guides/berlitz2/China-WhatToDo.txt
./written_2/travel_guides/berlitz2/China-WhereToGo.txt
./written_2/travel_guides/berlitz2/Costa-History.txt
./written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
./written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
./written_2/travel_guides/berlitz2/CostaBlanca-History.txt
./written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
./written_2/travel_guides/berlitz2/Crete-History.txt
./written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
./written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
./written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
./written_2/travel_guides/berlitz2/Cuba-History.txt
./written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
./written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
./written_2/travel_guides/berlitz2/Nepal-History.txt
./written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
./written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
./written_2/travel_guides/berlitz2/NewOrleans-History.txt
./written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
./written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
./written_2/travel_guides/berlitz2/Poland-History.txt
./written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
./written_2/travel_guides/berlitz2/Portugal-History.txt
./written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
./written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
./written_2/travel_guides/berlitz2/PuertoRico-History.txt
./written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
./written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
./written_2/travel_guides/berlitz2/Vallarta-History.txt
./written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
./written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
./written_2/demoResults.txt
./demoResults.txt
./grepResults.txt
./something.txt
```
## 4. `find /tmp -type f -name ".*"`

Finds all hidden files. I did this on the skill-demo1-data directory and got the following output: 

`find /tmp -type f -name ".*"` output:
```find: '/tmp/cs120wi23mm-pulse': Permission denied
find: '/tmp/cs120wi23al-pulse': Permission denied
find: '/tmp/yuw571-pulse': Permission denied
find: '/tmp/srustagi-pulse': Permission denied
find: '/tmp/cs15lwi23awd-pulse': Permission denied
find: '/tmp/cs120wi23ii-pulse': Permission denied
find: '/tmp/h7shi-pulse': Permission denied
find: '/tmp/cs120wi23ni-pulse': Permission denied
find: '/tmp/ee15wi23an-pulse': Permission denied
find: '/tmp/ee15wi23gf-pulse': Permission denied
find: '/tmp/cs15lwi23aik-pulse': Permission denied
find: '/tmp/cs120wi23aj-pulse': Permission denied
find: '/tmp/cs120wi23ej-pulse': Permission denied
find: '/tmp/cs15lwi23aqw-pulse': Permission denied
find: '/tmp/cs15lwi23aoz-pulse': Permission denied
find: '/tmp/cs120wi23gu-pulse': Permission denied
find: '/tmp/vscode-goWjd8rx': Permission denied
find: '/tmp/cs120wi23ip-pulse': Permission denied
find: '/tmp/cs120wi23js-pulse': Permission denied
find: '/tmp/cs15lwi23ta11-pulse': Permission denied
find: '/tmp/cs120wi23eu-pulse': Permission denied
find: '/tmp/hsperfdata_cs15lwi23ta3': Permission denied
find: '/tmp/cs15lwi23ani-pulse': Permission denied
find: '/tmp/cs120wi23lu-pulse': Permission denied
find: '/tmp/cs15lwi23apv-pulse': Permission denied
find: '/tmp/cs15lwi23anm-pulse': Permission denied
find: '/tmp/cs15lwi23aar-pulse': Permission denied
find: '/tmp/tmux-11283': Permission denied
find: '/tmp/cs15lwi23ahu-pulse': Permission denied
find: '/tmp/cs120wi23ek-pulse': Permission denied
find: '/tmp/cs120wi23mn-pulse': Permission denied
find: '/tmp/cs15lwi23amy-pulse': Permission denied
find: '/tmp/cs120wi23ax-pulse': Permission denied
find: '/tmp/ehammado-pulse': Permission denied
find: '/tmp/cs120wi23go-pulse': Permission denied
find: '/tmp/cs15lwi23ale-pulse': Permission denied
find: '/tmp/cs15lwi23abm-pulse': Permission denied
find: '/tmp/cs15lwi23awm-pulse': Permission denied
find: '/tmp/cs120wi23ks-pulse': Permission denied
find: '/tmp/cs120wi23ep-pulse': Permission denied
find: '/tmp/ssh-1ztV5oeqWGH3': Permission denied
find: '/tmp/cs120wi23gz-pulse': Permission denied
find: '/tmp/cs120wi23bb-pulse': Permission denied
find: '/tmp/cs120wi23fx-pulse': Permission denied
find: '/tmp/cs15lwi23asr-pulse': Permission denied
find: '/tmp/cs120wi23iq-pulse': Permission denied
find: '/tmp/cs120wi23ka-pulse': Permission denied
find: '/tmp/cs120wi23mt-pulse': Permission denied
find: '/tmp/cs15lwi23ahy-pulse': Permission denied
find: '/tmp/rmccrystal-pulse': Permission denied
find: '/tmp/cs15lwi23agd-pulse': Permission denied
find: '/tmp/cs15lwi23aot-pulse': Permission denied
find: '/tmp/cs120wi23hd-pulse': Permission denied
find: '/tmp/cs120wi23fm-pulse': Permission denied
find: '/tmp/cs15lwi23adl-pulse': Permission denied
find: '/tmp/cs15lwi23aad-pulse': Permission denied
find: '/tmp/cs15lwi23akl-pulse': Permission denied
find: '/tmp/cs120wi23qh-pulse': Permission denied
find: '/tmp/go-build763539080': Permission denied
find: '/tmp/ssh-rcigGTXCuhqF': Permission denied
find: '/tmp/cs120wi23ls-pulse': Permission denied
find: '/tmp/cs120wi23cf-pulse': Permission denied
find: '/tmp/tmux-106755': Permission denied
find: '/tmp/cs15lwi23aev-pulse': Permission denied
find: '/tmp/cs120wi23og-pulse': Permission denied
find: '/tmp/cs15lwi23auz-pulse': Permission denied
find: '/tmp/cs15lwi23anh-pulse': Permission denied
find: '/tmp/cs15lwi23ahc-pulse': Permission denied
find: '/tmp/cs120wi23aa-pulse': Permission denied
find: '/tmp/cs15lwi23aqx-pulse': Permission denied
find: '/tmp/cs120wi23at-pulse': Permission denied
find: '/tmp/cs120wi23eq-pulse': Permission denied
find: '/tmp/cs120wi23cd-pulse': Permission denied
find: '/tmp/cs120wi23pe-pulse': Permission denied
find: '/tmp/tmux-11918': Permission denied
find: '/tmp/cs15lwi23aio-pulse': Permission denied
find: '/tmp/adsampat-pulse': Permission denied
find: '/tmp/cs15lwi23acs-pulse': Permission denied
find: '/tmp/cs120wi23ob-pulse': Permission denied
find: '/tmp/ee15wi23av-pulse': Permission denied
find: '/tmp/cs15lwi23amt-pulse': Permission denied
find: '/tmp/cs120wi23li-pulse': Permission denied
find: '/tmp/cs120wi23es-pulse': Permission denied
find: '/tmp/cs15lwi23alg-pulse': Permission denied
find: '/tmp/ee15wi23ta1-pulse': Permission denied
find: '/tmp/cs120wi23cp-pulse': Permission denied
find: '/tmp/cs120wi23kb-pulse': Permission denied
find: '/tmp/cs120wi23as-pulse': Permission denied
find: '/tmp/cs15lwi23akh-pulse': Permission denied
find: '/tmp/cs15lwi23amv-pulse': Permission denied
find: '/tmp/cs120wi23ew-pulse': Permission denied
find: '/tmp/cs120wi23mz-pulse': Permission denied
find: '/tmp/cs120wi23lo-pulse': Permission denied
find: '/tmp/cs120wi23ll-pulse': Permission denied
find: '/tmp/cs120wi23fu-pulse': Permission denied
find: '/tmp/cs120wi23mf-pulse': Permission denied
find: '/tmp/cs15lwi23add-pulse': Permission denied
find: '/tmp/systemd-private-6671687ec48e42eea89967aef55de198-ntpd.service-WAxIZA': Permission denied
find: '/tmp/cs15lwi23agi-pulse': Permission denied
find: '/tmp/cs15lwi23anl-pulse': Permission denied
find: '/tmp/cs15lwi23asc-pulse': Permission denied
find: '/tmp/cs120wi23fw-pulse': Permission denied
find: '/tmp/cs15lwi23ajb-pulse': Permission denied
find: '/tmp/cs15lwi23acd-pulse': Permission denied
find: '/tmp/cs120wi23hz-pulse': Permission denied
find: '/tmp/cs120wi23hs-pulse': Permission denied
find: '/tmp/cs15lwi23ahp-pulse': Permission denied
find: '/tmp/gopls-18048.1': Permission denied
find: '/tmp/cs120wi23fd-pulse': Permission denied
find: '/tmp/cs120wi23jv-pulse': Permission denied
find: '/tmp/cs120wi23kc-pulse': Permission denied
find: '/tmp/cs120wi23qg-pulse': Permission denied
find: '/tmp/cs120wi23pk-pulse': Permission denied
find: '/tmp/ee15wi23ex-pulse': Permission denied
find: '/tmp/cs15lwi23avo-pulse': Permission denied
find: '/tmp/cs120wi23lf-pulse': Permission denied
find: '/tmp/cs120wi23kf-pulse': Permission denied
find: '/tmp/cs15lwi23aol-pulse': Permission denied
find: '/tmp/cs15lwi23anc-pulse': Permission denied
find: '/tmp/cs120wi23ox-pulse': Permission denied
find: '/tmp/cs15lwi23agt-pulse': Permission denied
find: '/tmp/cs120wi23bp-pulse': Permission denied
find: '/tmp/tmux-110418': Permission denied
find: '/tmp/cs15lwi23aes-pulse': Permission denied
find: '/tmp/cs15lwi23amd-pulse': Permission denied
find: '/tmp/cs15lwi23ta15-pulse': Permission denied
find: '/tmp/cs15lwi23acw-pulse': Permission denied
find: '/tmp/cs120wi23fq-pulse': Permission denied
find: '/tmp/cs120wi23ie-pulse': Permission denied
find: '/tmp/hsperfdata_cs15lwi23ta9': Permission denied
find: '/tmp/cs120wi23de-pulse': Permission denied
find: '/tmp/cs120wi23nb-pulse': Permission denied
find: '/tmp/cs15lwi23arn-pulse': Permission denied
find: '/tmp/cs120wi23lr-pulse': Permission denied
find: '/tmp/cs15lwi23aup-pulse': Permission denied
find: '/tmp/gopls-9417.1': Permission denied
find: '/tmp/cs15lwi23apr-pulse': Permission denied
find: '/tmp/tmux-11526': Permission denied
find: '/tmp/cs120wi23os-pulse': Permission denied
find: '/tmp/cs120wi23op-pulse': Permission denied
find: '/tmp/cs120wi23dj-pulse': Permission denied
find: '/tmp/vchase-pulse': Permission denied
find: '/tmp/cs15lwi23amq-pulse': Permission denied
find: '/tmp/cs15lwi23acc-pulse': Permission denied
find: '/tmp/aag011-pulse': Permission denied
find: '/tmp/cs15lwi23aeg-pulse': Permission denied
find: '/tmp/cs15lwi23acn-pulse': Permission denied
find: '/tmp/tmux-123194': Permission denied
find: '/tmp/cs120wi23jd-pulse': Permission denied
find: '/tmp/cs120wi23fj-pulse': Permission denied
find: '/tmp/cs15lwi23atp-pulse': Permission denied
find: '/tmp/cs15lwi23aqo-pulse': Permission denied
find: '/tmp/hsperfdata_cs15lwi23ta6': Permission denied
find: '/tmp/ee15wi23zz-pulse': Permission denied
find: '/tmp/cs15lwi23aac-pulse': Permission denied
find: '/tmp/cs15lwi23agy-pulse': Permission denied
find: '/tmp/cs15lwi23alw-pulse': Permission denied
find: '/tmp/cs15lwi23akm-pulse': Permission denied
find: '/tmp/cs120wi23ex-pulse': Permission denied
find: '/tmp/cs15lwi23ta9-pulse': Permission denied
find: '/tmp/cs120wi23ih-pulse': Permission denied
find: '/tmp/cs120wi23cv-pulse': Permission denied
find: '/tmp/cs120wi23bd-pulse': Permission denied
find: '/tmp/cs120wi23by-pulse': Permission denied
find: '/tmp/cs120wi23ca-pulse': Permission denied
find: '/tmp/cs120wi23dv-pulse': Permission denied
find: '/tmp/cs120wi23ng-pulse': Permission denied
find: '/tmp/cs120wi23dk-pulse': Permission denied
find: '/tmp/cs15lwi23age-pulse': Permission denied
find: '/tmp/cs120wi23ij-pulse': Permission denied
find: '/tmp/dyeung-pulse': Permission denied
find: '/tmp/cs120wi23zz-pulse': Permission denied
find: '/tmp/cs120wi23pz-pulse': Permission denied
find: '/tmp/cs15lwi23atd-pulse': Permission denied
find: '/tmp/cs120wi23kt-pulse': Permission denied
find: '/tmp/cs15lwi23alz-pulse': Permission denied
find: '/tmp/cs120wi23ln-pulse': Permission denied
find: '/tmp/cs120wi23cr-pulse': Permission denied
find: '/tmp/yaw048-pulse': Permission denied
find: '/tmp/ee15wi23hn-pulse': Permission denied
find: '/tmp/cs120wi23gr-pulse': Permission denied
find: '/tmp/cs15lwi23ta13-pulse': Permission denied
find: '/tmp/cs15lwi23afs-pulse': Permission denied
find: '/tmp/cs15lwi23axq-pulse': Permission denied
find: '/tmp/ssh-nbBdWFWks1c2': Permission denied
find: '/tmp/cs15lwi23aov-pulse': Permission denied
find: '/tmp/cs120wi23ml-pulse': Permission denied
find: '/tmp/tmux-105140': Permission denied
find: '/tmp/cs15lwi23akw-pulse': Permission denied
find: '/tmp/cs120wi23jp-pulse': Permission denied
find: '/tmp/cs120wi23lh-pulse': Permission denied
find: '/tmp/cs15lwi23aui-pulse': Permission denied
find: '/tmp/cs120wi23hk-pulse': Permission denied
find: '/tmp/ee15wi23ai-pulse': Permission denied
find: '/tmp/cs15lwi23akt-pulse': Permission denied
find: '/tmp/cs15lwi23aoa-pulse': Permission denied
find: '/tmp/cs120wi23cs-pulse': Permission denied
find: '/tmp/cs120wi23fn-pulse': Permission denied
find: '/tmp/cs120wi23fb-pulse': Permission denied
find: '/tmp/cs120wi23ds-pulse': Permission denied
find: '/tmp/cs15lwi23aao-pulse': Permission denied
find: '/tmp/cs120wi23nz-pulse': Permission denied
find: '/tmp/cs120wi23ao-pulse': Permission denied
find: '/tmp/cs15lwi23amb-pulse': Permission denied
find: '/tmp/cs120wi23jl-pulse': Permission denied
find: '/tmp/cs15lwi23apm-pulse': Permission denied
find: '/tmp/chz043-pulse': Permission denied
find: '/tmp/cs120wi23ha-pulse': Permission denied
find: '/tmp/cs15lwi23asi-pulse': Permission denied
find: '/tmp/cs15lwi23adz-pulse': Permission denied
find: '/tmp/cs120wi23bi-pulse': Permission denied
find: '/tmp/cs120wi23io-pulse': Permission denied
find: '/tmp/cs120wi23mr-pulse': Permission denied
find: '/tmp/cs15lwi23aje-pulse': Permission denied
find: '/tmp/cs120wi23an-pulse': Permission denied
find: '/tmp/cs120wi23ci-pulse': Permission denied
find: '/tmp/xpang-pulse': Permission denied
find: '/tmp/cs120wi23jn-pulse': Permission denied
find: '/tmp/cs15lwi23ta12-pulse': Permission denied
find: '/tmp/cs15lwi23ams-pulse': Permission denied
find: '/tmp/jgeng-pulse': Permission denied
find: '/tmp/cs15lwi23aub-pulse': Permission denied
find: '/tmp/cs120wi23ff-pulse': Permission denied
find: '/tmp/cs120wi23hj-pulse': Permission denied
find: '/tmp/cs15lwi23agg-pulse': Permission denied
find: '/tmp/cs15lwi23akg-pulse': Permission denied
find: '/tmp/cs120wi23gg-pulse': Permission denied
find: '/tmp/cs15lwi23auk-pulse': Permission denied
find: '/tmp/cs15lwi23app-pulse': Permission denied
find: '/tmp/cs15lwi23acu-pulse': Permission denied
find: '/tmp/cs120wi23da-pulse': Permission denied
find: '/tmp/cs15lwi23aps-pulse': Permission denied
find: '/tmp/cs15lwi23abg-pulse': Permission denied
find: '/tmp/cs120wi23jy-pulse': Permission denied
find: '/tmp/cs120wi23cg-pulse': Permission denied
find: '/tmp/cs120wi23dy-pulse': Permission denied
find: '/tmp/cs15lwi23amn-pulse': Permission denied
find: '/tmp/cs120wi23gv-pulse': Permission denied
find: '/tmp/cs15lwi23akn-pulse': Permission denied
find: '/tmp/cs15lwi23atn-pulse': Permission denied
find: '/tmp/cs15lwi23abu-pulse': Permission denied
find: '/tmp/cs15lwi23auu-pulse': Permission denied
find: '/tmp/go-build3720618972': Permission denied
find: '/tmp/cs15lwi23ant-pulse': Permission denied
find: '/tmp/cs120wi23cw-pulse': Permission denied
find: '/tmp/cs120wi23ho-pulse': Permission denied
find: '/tmp/cs15lwi23aed-pulse': Permission denied
find: '/tmp/cs120wi23gj-pulse': Permission denied
find: '/tmp/cs120wi23ae-pulse': Permission denied
find: '/tmp/cs15lwi23aid-pulse': Permission denied
find: '/tmp/cs15lwi23aka-pulse': Permission denied
find: '/tmp/ssh-hqk5MOoki7E4': Permission denied
find: '/tmp/cs120wi23gl-pulse': Permission denied
find: '/tmp/ee15wi23af-pulse': Permission denied
find: '/tmp/cs15lwi23amj-pulse': Permission denied
find: '/tmp/cs15lwi23aob-pulse': Permission denied
find: '/tmp/calee-pulse': Permission denied
find: '/tmp/cs15lwi23aua-pulse': Permission denied
find: '/tmp/cs15lwi23abo-pulse': Permission denied
find: '/tmp/cs15lwi23aaq-pulse': Permission denied
find: '/tmp/jiz188-pulse': Permission denied
find: '/tmp/cs120wi23be-pulse': Permission denied
find: '/tmp/dmvo-pulse': Permission denied
find: '/tmp/vscode-go38kl4v': Permission denied
find: '/tmp/cs120wi23hb-pulse': Permission denied
find: '/tmp/hsperfdata_cs15lwi23ta13': Permission denied
find: '/tmp/cs15lwi23aru-pulse': Permission denied
find: '/tmp/cs15lwi23agp-pulse': Permission denied
find: '/tmp/ruc003-pulse': Permission denied
find: '/tmp/cs15lwi23aqt-pulse': Permission denied
find: '/tmp/cs120wi23od-pulse': Permission denied
find: '/tmp/cs120wi23ec-pulse': Permission denied
find: '/tmp/cs15lwi23atq-pulse': Permission denied
find: '/tmp/cs120wi23hh-pulse': Permission denied
find: '/tmp/cs120wi23bg-pulse': Permission denied
find: '/tmp/cs120wi23bm-pulse': Permission denied
find: '/tmp/cs120wi23ly-pulse': Permission denied
find: '/tmp/cs15lwi23afv-pulse': Permission denied
find: '/tmp/cs15lwi23aiy-pulse': Permission denied
find: '/tmp/cs120wi23gw-pulse': Permission denied
find: '/tmp/cs15lwi23amo-pulse': Permission denied
find: '/tmp/cs15lwi23aso-pulse': Permission denied
find: '/tmp/cs120wi23ab-pulse': Permission denied
find: '/tmp/cs120wi23ns-pulse': Permission denied
find: '/tmp/ee15wi23-pulse': Permission denied
find: '/tmp/cs15lwi23atg-pulse': Permission denied
find: '/tmp/cs15lwi23aul-pulse': Permission denied
find: '/tmp/cs120wi23ia-pulse': Permission denied
find: '/tmp/cs120wi23pd-pulse': Permission denied
find: '/tmp/cs120wi23du-pulse': Permission denied
find: '/tmp/cs120wi23hl-pulse': Permission denied
find: '/tmp/cs120wi23qd-pulse': Permission denied
find: '/tmp/cs15lwi23ahi-pulse': Permission denied
find: '/tmp/cs15lwi23alr-pulse': Permission denied
find: '/tmp/cs15lwi23afq-pulse': Permission denied
find: '/tmp/hsperfdata_cs15lwi23ta11': Permission denied
find: '/tmp/ffgutierrez-pulse': Permission denied
find: '/tmp/cs15lwi23ave-pulse': Permission denied
find: '/tmp/cs120wi23am-pulse': Permission denied
find: '/tmp/cs120wi23ak-pulse': Permission denied
find: '/tmp/cs15lwi23aja-pulse': Permission denied
find: '/tmp/cs15lwi23aoe-pulse': Permission denied
find: '/tmp/cs15lwi23avh-pulse': Permission denied
find: '/tmp/cs120wi23lj-pulse': Permission denied
find: '/tmp/cs15lwi23awu-pulse': Permission denied
find: '/tmp/cs120wi23ta6-pulse': Permission denied
find: '/tmp/cs15lwi23ta3-pulse': Permission denied
find: '/tmp/cs120wi23nq-pulse': Permission denied
find: '/tmp/cs120wi23bz-pulse': Permission denied
find: '/tmp/ee15wi23bs-pulse': Permission denied
find: '/tmp/cs15lwi23aaw-pulse': Permission denied
find: '/tmp/cs120wi23ei-pulse': Permission denied
find: '/tmp/cs120wi23je-pulse': Permission denied
find: '/tmp/cs15lwi23abi-pulse': Permission denied
find: '/tmp/cs15lwi23ado-pulse': Permission denied
find: '/tmp/cs120wi23lx-pulse': Permission denied
find: '/tmp/cs120wi23hr-pulse': Permission denied
find: '/tmp/cs15lwi23adi-pulse': Permission denied
find: '/tmp/cs15lwi23aet-pulse': Permission denied
find: '/tmp/cs120wi23oh-pulse': Permission denied
find: '/tmp/ee15wi23fo-pulse': Permission denied
find: '/tmp/cs15lwi23afn-pulse': Permission denied
find: '/tmp/psyeh-pulse': Permission denied
find: '/tmp/cs15lwi23alb-pulse': Permission denied
find: '/tmp/cs120wi23af-pulse': Permission denied
find: '/tmp/cs15lwi23aqv-pulse': Permission denied
find: '/tmp/cs120wi23pm-pulse': Permission denied
find: '/tmp/cs120wi23ig-pulse': Permission denied
find: '/tmp/cs120wi23-pulse': Permission denied
find: '/tmp/cs15lwi23atx-pulse': Permission denied
find: '/tmp/cs15lwi23aky-pulse': Permission denied
find: '/tmp/cs120wi23he-pulse': Permission denied
find: '/tmp/cs15lwi23ta6-pulse': Permission denied
find: '/tmp/cs120wi23kw-pulse': Permission denied
find: '/tmp/cs120wi23ph-pulse': Permission denied
``` 
Clearly, there were many hidden files that I was not able to access, but at least with this command now I know it exists.

Sources: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/
https://www.tecmint.com/35-practical-examples-of-linux-find-command/
