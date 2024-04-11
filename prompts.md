Você é um assistente de previsão de séries temporais e eu vou passar para você uma série temporal oriunda da linha 3 de ônibus da cidade de Fortaleza. Será lhe passado um JSON contendo dados de 60 dias da linha 3, o JSON inicia com a primeira chave representando os meses e dentro da chave temos os dias daquele mês, na chave dia temos uma chave que representa o dia da semana (0 - domingo, 1 - segunda, 2 - terça, 3 - quarta, 4 - quinta, 5 - sexta, 6 sábado), em seguida temos uma que representa a quantidade de passageiros que foram em cada hora daquele dia e por fim uma chave que indica se é feriado ou não nesse dia.

Cada valor da chave passageiros representa a quantidade de passageiros que entrou em um determinado horário naquele dia, cada valor seguinte representa uma hora incrementada, ou seja, o próximo dado é referente às 02 horas da manhã e assim sucessivamente. Seu objetivo é prever a quantidade de passageiros que utilizarão a linha nas próximas N horas solicitadas. O formato da sua saída deve ser apenas de uma lista com os N valores solicitados. Em hipótese alguma explique a sua solução ou adicione qualquer texto no início e final da lista. Informe a sequência de números só com N números previstos, não inclusos os números anteriores que você utilizou para fazer sua previsão.

A sequência que você deve continuar é:

{
    "1": {
        "1": {
            "dia_semana": 0,
            "passageiros": "5,24,23,24,64,258,209,196,209,200,155,130,156,222,235,337,447,391,422,249,211,166,41",
            "feriado": 1
        },
        "2": {
            "dia_semana": 1,
            "passageiros": "6,3,12,5,108,303,595,463,479,513,625,697,663,690,739,876,1083,1157,1121,914,627,501,686,82",
            "feriado": 0
        },
        "3": {
            "dia_semana": 2,
            "passageiros": "22,12,5,3,56,251,525,464,390,430,551,774,767,751,879,909,978,1188,1150,943,687,506,659,66",
            "feriado": 0
        },
        "4": {
            "dia_semana": 3,
            "passageiros": "23,4,4,2,68,256,465,422,413,452,555,724,809,723,777,792,1083,1187,1144,950,655,523,554,73",
            "feriado": 0
        },
        "5": {
            "dia_semana": 4,
            "passageiros": "24,7,9,6,62,245,479,445,418,491,654,806,907,810,914,1023,1251,1251,1202,1043,753,551,630,87",
            "feriado": 0
        },
        "6": {
            "dia_semana": 5,
            "passageiros": "22,15,5,7,62,163,274,334,396,397,506,630,763,705,814,924,951,996,1038,886,846,713,726,104",
            "feriado": 0
        },
        "7": {
            "dia_semana": 6,
            "passageiros": "30,15,9,12,28,95,149,204,165,183,219,253,262,241,332,464,707,671,867,766,690,733,245,50",
            "feriado": 0
        },
        "8": {
            "dia_semana": 0,
            "passageiros": "15,5,10,8,126,353,605,574,514,507,716,879,941,885,906,1072,1255,1407,1270,1214,1052,795,747,112",
            "feriado": 0
        },
        "9": {
            "dia_semana": 1,
            "passageiros": "33,2,6,5,55,258,529,493,382,487,635,785,844,768,824,903,1045,1330,1254,951,718,505,597,60",
            "feriado": 0
        },
        "10": {
            "dia_semana": 2,
            "passageiros": "15,5,6,3,58,274,523,449,422,417,550,738,648,677,811,942,1098,1373,1230,927,675,515,583,78",
            "feriado": 0
        },
        "11": {
            "dia_semana": 3,
            "passageiros": "18,14,9,4,44,271,503,430,405,418,532,767,761,677,798,847,1045,1253,1152,920,706,474,596,78",
            "feriado": 0
        },
        "12": {
            "dia_semana": 4,
            "passageiros": "29,6,8,1,68,252,498,452,398,414,561,736,734,668,768,851,1089,1253,1228,876,711,506,642,70",
            "feriado": 0
        },
        "13": {
            "dia_semana": 5,
            "passageiros": "20,19,7,7,69,191,330,314,362,353,481,676,756,697,702,793,1004,923,964,901,815,666,738,72",
            "feriado": 0
        },
        "14": {
            "dia_semana": 6,
            "passageiros": "23,13,10,8,43,104,147,166,177,164,227,237,182,254,321,453,707,778,771,726,648,709,217,42",
            "feriado": 0
        },
        "15": {
            "dia_semana": 0,
            "passageiros": "29,4,13,9,114,386,649,590,498,486,649,834,804,785,815,931,1112,1506,1458,1187,990,754,781,77",
            "feriado": 0
        },
        "16": {
            "dia_semana": 1,
            "passageiros": "48,5,6,2,52,294,519,468,417,423,659,833,795,736,874,878,1030,1272,1191,989,705,589,640,66",
            "feriado": 0
        },
        "17": {
            "dia_semana": 2,
            "passageiros": "16,7,7,6,60,273,524,453,403,379,626,768,727,738,776,832,1015,1323,1217,798,673,601,627,65",
            "feriado": 0
        },
        "18": {
            "dia_semana": 3,
            "passageiros": "14,8,6,7,56,266,441,437,382,403,521,739,721,706,742,886,991,1237,1092,827,607,470,633,69",
            "feriado": 0
        },
        "19": {
            "dia_semana": 4,
            "passageiros": "16,7,10,6,62,254,452,384,460,359,532,708,722,763,820,908,1109,1272,1322,1005,786,574,652,77",
            "feriado": 0
        },
        "20": {
            "dia_semana": 5,
            "passageiros": "17,23,6,6,50,197,314,311,331,371,496,657,706,691,700,764,895,1070,1035,879,915,603,795,88",
            "feriado": 0
        },
        "21": {
            "dia_semana": 6,
            "passageiros": "16,18,17,9,38,91,144,153,177,201,206,231,217,262,337,546,598,776,822,704,600,743,269,45",
            "feriado": 0
        },
        "22": {
            "dia_semana": 0,
            "passageiros": "17,12,5,8,129,381,647,571,529,496,550,860,805,799,816,1008,1179,1549,1392,1080,863,704,786,98",
            "feriado": 0
        },
        "23": {
            "dia_semana": 1,
            "passageiros": "37,3,4,4,65,293,526,478,430,395,607,736,758,671,773,890,983,1294,1193,790,628,400,587,55",
            "feriado": 0
        },
        "24": {
            "dia_semana": 2,
            "passageiros": "15,8,4,2,64,282,475,434,383,384,557,679,698,665,719,825,975,1228,1147,769,623,456,588,57",
            "feriado": 0
        },
        "25": {
            "dia_semana": 3,
            "passageiros": "17,5,3,13,60,274,489,456,355,383,490,687,660,660,712,891,1091,1171,1151,835,574,468,621,59",
            "feriado": 0
        },
        "26": {
            "dia_semana": 4,
            "passageiros": "21,16,7,6,64,276,471,529,404,368,561,686,805,662,798,939,1069,1235,1173,938,720,537,702,68",
            "feriado": 0
        },
        "27": {
            "dia_semana": 5,
            "passageiros": "15,19,6,9,48,186,296,341,322,326,431,519,604,547,590,659,771,698,809,657,573,421,667,61",
            "feriado": 0
        },
        "28": {
            "dia_semana": 6,
            "passageiros": "37,14,4,9,52,96,127,186,158,140,175,246,198,271,386,510,686,806,725,761,595,664,241,37",
            "feriado": 0
        },
        "29": {
            "dia_semana": 0,
            "passageiros": "19,11,4,9,120,404,580,574,520,512,595,832,799,674,730,914,1210,1267,1257,950,669,537,722,86",
            "feriado": 0
        },
        "30": {
            "dia_semana": 1,
            "passageiros": "17,9,1,4,52,304,518,526,401,447,528,768,738,685,837,904,1034,1210,1071,824,679,457,590,66",
            "feriado": 0
        },
        "31": {
            "dia_semana": 2,
            "passageiros": "19,17,1,8,55,298,570,438,427,451,622,734,805,712,740,857,1079,1282,1292,845,747,506,618,69",
            "feriado": 0
        }
    },
    "2": {
        "1": {
            "dia_semana": 3,
            "passageiros": "15,14,3,10,52,330,588,478,415,464,586,822,748,697,786,964,1075,1256,1216,923,739,511,627,96",
            "feriado": 0
        },
        "2": {
            "dia_semana": 4,
            "passageiros": "10,10,7,7,71,305,606,548,424,445,607,784,876,831,870,971,1142,1315,1109,921,709,496,632,72",
            "feriado": 0
        },
        "3": {
            "dia_semana": 5,
            "passageiros": "20,12,7,8,49,203,287,309,372,398,488,737,890,789,775,843,977,1067,1053,953,866,575,690,104",
            "feriado": 0
        },
        "4": {
            "dia_semana": 6,
            "passageiros": "22,8,19,9,36,131,151,220,183,160,227,292,244,362,352,440,507,702,675,612,430,535,195,49",
            "feriado": 0
        },
        "5": {
            "dia_semana": 0,
            "passageiros": "17,9,11,7,100,455,689,680,562,469,605,705,851,837,871,1027,1286,1456,1331,993,866,683,705,91",
            "feriado": 0
        },
        "6": {
            "dia_semana": 1,
            "passageiros": "14,7,8,1,60,357,620,571,484,443,639,911,873,803,911,996,1163,1450,1338,981,742,623,682,64",
            "feriado": 0
        },
        "7": {
            "dia_semana": 2,
            "passageiros": "18,5,2,9,61,299,654,534,468,456,559,872,840,788,903,1001,1299,1457,1243,1030,830,652,705,81",
            "feriado": 0
        },
        "8": {
            "dia_semana": 3,
            "passageiros": "16,6,9,7,60,343,666,532,445,488,616,804,972,799,801,982,1163,1325,1367,973,800,551,714,93",
            "feriado": 0
        },
        "9": {
            "dia_semana": 4,
            "passageiros": "19,13,6,8,59,308,588,516,456,461,548,715,891,855,882,997,1302,1326,1311,1031,814,671,837,80",
            "feriado": 0
        },
        "10": {
            "dia_semana": 5,
            "passageiros": "26,8,9,7,52,185,243,262,201,253,379,529,622,566,618,674,774,835,778,668,645,669,549,64",
            "feriado": 0
        },
        "11": {
            "dia_semana": 6,
            "passageiros": "20,7,5,6,35,85,141,154,148,158,166,154,123,151,204,303,357,350,335,242,211,112,167,50",
            "feriado": 0
        },
        "12": {
            "dia_semana": 0,
            "passageiros": "14,12,4,1,37,111,195,188,105,121,136,162,140,218,248,277,383,427,364,355,488,339,275,41",
            "feriado": 1
        },
        "13": {
            "dia_semana": 1,
            "passageiros": "13,7,8,2,25,79,154,158,181,189,200,168,199,173,313,282,390,503,372,326,515,148,218,46",
            "feriado": 1
        },
        "14": {
            "dia_semana": 2,
            "passageiros": "9,8,14,3,34,193,296,299,249,294,318,400,483,591,661,781,970,943,938,608,399,309,535,48",
            "feriado": 0
        },
        "15": {
            "dia_semana": 3,
            "passageiros": "7,5,15,2,83,349,539,522,425,440,615,768,820,753,895,871,1223,1345,1272,925,739,631,647,85",
            "feriado": 0
        },
        "16": {
            "dia_semana": 4,
            "passageiros": "23,9,11,5,63,296,581,524,415,409,583,788,828,803,869,982,1202,1336,1320,1043,714,633,683,61",
            "feriado": 0
        },
        "17": {
            "dia_semana": 5,
            "passageiros": "22,15,6,4,46,172,301,312,272,269,367,543,697,577,672,825,949,1029,944,887,701,611,642,67",
            "feriado": 0
        },
        "18": {
            "dia_semana": 6,
            "passageiros": "31,21,7,6,36,85,129,164,158,168,183,241,166,266,335,471,649,724,793,675,644,727,204,42",
            "feriado": 0
        },
        "19": {
            "dia_semana": 0,
            "passageiros": "14,8,4,6,112,394,802,614,603,526,634,802,878,757,826,1002,1219,1424,1424,1063,719,727,776,86",
            "feriado": 0
        },
        "20": {
            "dia_semana": 1,
            "passageiros": "58,11,6,3,54,339,680,578,474,439,700,848,914,792,794,881,1143,1332,1257,1010,748,660,730,89",
            "feriado": 0
        },
        "21": {
            "dia_semana": 2,
            "passageiros": "23,6,9,13,59,293,664,534,428,498,603,754,745,667,765,798,1088,1320,1263,793,656,611,749,74",
            "feriado": 0
        },
        "22": {
            "dia_semana": 3,
            "passageiros": "26,9,7,7,62,328,693,521,394,367,562,701,764,743,727,924,1087,1276,1175,737,569,551,689,75",
            "feriado": 0
        },
        "23": {
            "dia_semana": 4,
            "passageiros": "22,8,12,4,57,321,628,508,441,469,602,766,886,689,814,833,1042,1279,1176,876,623,585,724,86",
            "feriado": 0
        },
        "24": {
            "dia_semana": 5,
            "passageiros": "24,15,11,6,42,199,311,372,354,333,480,668,755,707,698,708,957,908,961,874,740,560,660,80",
            "feriado": 0
        },
        "25": {
            "dia_semana": 6,
            "passageiros": "20,11,11,4,50,113,150,220,144,127,181,199,255,283,344,414,682,710,683,660,596,598,247,43",
            "feriado": 0
        },
        "26": {
            "dia_semana": 0,
            "passageiros": "21,7,10,22,100,460,819,630,620,518,725,891,979,778,818,908,1197,1412,1302,910,675,742,834,85",
            "feriado": 0
        },
        "27": {
            "dia_semana": 1,
            "passageiros": "20,1,2,49,297,697,540,460,481,702,948,873,810,811,807,1115,1291,1197,788,585,561,694,77",
            "feriado": 0
        },
        "28": {
            "dia_semana": 2,
            "passageiros": "13,6,1,14,54,332,674,522,484,482,723,938,884,779,822,931,1191,1308,1259,840,713,626,734,77",
            "feriado": 0
        }
    },
    "3": {
        "1": {
            "dia_semana": 3,
            "passageiros": "11,9,4,9,60,315,667,518,420,441,685,839,832,698,760,762,1023,1243,1282,846,678,636,677,95",
            "feriado": 0
        },
        "2": {
            "dia_semana": 4,
            "passageiros": "21,11",
            "feriado": 0
        }
    }
}

preveja os próximos 144 números da sequência: