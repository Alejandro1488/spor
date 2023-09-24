# spor

вариант2 деньги

import _ from 'lodash';

export default (content) => {
  // Write your code here
  const data = content.split('\n').slice(1, -1).map((row) => row.split(';'));
  console.log(`Count: ${data.length}`)
// step 2
const letterCode = data.map((row) => (row[3]));
const sortedLetter = _.uniq(letterCode).sort().join(', ')
console.log(Currency codes: ${sortedLetter})

// step 3
const rate = data.map((row) => Number(row[4]));
const maxRate = Math.max(...rate);
const minRate = Math.min(...rate)
 console.log(Cost of currency: Min: ${minRate}, Max: ${maxRate});

//step 4
const countInRange = rate.filter((value) => value >= 10 && value <= 30).length;
console.log(Count currency between 10 and 30: ${countInRange});
}


вариант3 автомобили

import _ from 'lodash';
export default (content) => {
const data = content.split('\n').slice(1, -1).map((row) => row.split(','));
console.log(Количество автомобилей: ${data.length})
//step 2
const dataMileage = data.map((row) => Number(row[4]));
const dataSorted = _.mean(dataMileage);
console.log(Средний пробег: ${Math.round(dataSorted)})
//step 3 
const maxCost = data.map((row) => Number(row[7]))
const maxCount = _.max(maxCost)
console.log(Стоимость самой дорогой машины: ${maxCount});
//step 4
const maxOldest = _.minBy(data, (row) => Number(row[2]))
console.log(Самый старый автомобиль: ${maxOldest[0]} ${maxOldest[1]})
}


вариант 6 планеты

// node bin/stars.js fixtures/stars1.csv
import _ from 'lodash';
export default (content) =>{
const rows = content.split('\n').slice(2)
const data = rows.map((row) => row.split('|').slice(1).slice(0, -1).map((row) => row.trim()))
console.log(Count: ${data.length});
//step 2
const galaxies = _.uniq(data.map((row) => row[1]).sort());
console.log(Galaxies: ${galaxies.join(', ')});
//step 3
const maxDist = _.max(data.map((row) => Number(row[4])));
const minDist = _.min(data.map((row) => Number(row[4])));
console.log(Farest from Earth: ${maxDist} light years, closest to Earth: ${minDist} light years);
//step 4
const closietGalaxy = _.minBy(data, (row) => Number(row[4]))
console.log(Closest to Earth: ${closietGalaxy[0]} in ${closietGalaxy[1]} galaxy);
}

вариант 7 города у меня


// node bin/money.js fixtures/currencies1.csv
запуск в терминале

npm i             make .....



node bin/money.js __fixtures__/currencies.csv

npm test   make test    npm ci lodash 





шпора фимы


import _ from 'lodash'

export default (content) => { 

    //  Первое задание
    const data = content.split('\n').slice(1); 
    console.log(`Количество рядов: ${data.length}`) 

    const make_hero = (content) => {
        const bobi = {race:content[0], stronge:parseInt(content[1]), health:content[2], division:parseInt(content[3]), hight:content[4], kg:parseInt(content[5]), price:content[6]}
        return bobi;
    };
         const rows = data.map((row) => row 
    .split('|') 
     .filter((row) => row)) 
    .map((array) => array  
        .map((element) => element.trim()) 
         ); 

    const jopa = rows.map((row) => make_hero(row));
    const jopa1 = jopa.map((row) => row.stronge);
    const jopa2 = Math.max(...jopa1);
    const jopa3 = jopa.filter((row) => row.stronge === jopa2);
    console.log(jopa3[0].price * 10);
    const jopa4 = jopa.filter((row) => row.stronge !== jopa2);
    const jopa5 = jopa4.map((row) => row.stronge);
    const jopa6 = Math.max(...jopa5);
    const jopa7 = jopa.filter((row) => row.stronge === jopa6)
    console.log(jopa7[0].price*20)

    const xui = jopa.map((row) => row.kg);
    const xui2 = Math.max(...xui);
    const xui3 = jopa.filter((row) => row.kg === xui2);
    const mintolstii = Math.min(...xui);
    const minkg = jopa.filter((row) => row.kg === mintolstii )
    console.log(xui3[0].price * xui3[0].division)
    console.log(minkg[0].price * minkg[0].division)


    // // Второе задание

    // const rows = data.map((row) => row 
    // .split('|') 
    // .filter((row) => row)) 
    // .map((array) => array  
    //     .map((element) => element.trim()) 
    //     ); 
 
    // const creatures = rows.map((row) => row[0]); 
    // const price = rows.map((row) => Number(row[6])); 
 
 
    // const strengths = rows.map((row) => Number(row[1])); 
    // const strongestIndex = strengths.indexOf(Math.max(...strengths)); 
    // const strengthsWithoutStrongest = strengths.slice(); 
    // strengthsWithoutStrongest[strongestIndex] = 0; 
    // const secondStrongestIndex = strengthsWithoutStrongest.indexOf(Math.max(...strengthsWithoutStrongest)); 
     
    // console.log(`цена за 10 сильнейших созданий: ${price[strongestIndex]*10}`); 
    // console.log(`цена за 20 вторых по силе созданий: ${price[secondStrongestIndex]*20}`);

    // // Третье задание

    // const unitsInDivision = rows.map((row) => row[3])
    // const averageWeight = rows.map((row) => Number(row[5]));
    // const fattestUnit = averageWeight.indexOf(Math.max(...averageWeight));
    // const fattesThinestUnit = averageWeight.indexOf(Math.min(...averageWeight));

    // console.log(`цена за отряд самых толстых: ${price[fattestUnit]}`);
    // console.log(`цена за отряд самых худых: ${}`);


}




https://selectel.ru/blog/tutorials/how-to-generate-ssh/
ключ








Как сгенерировать SSH-ключ для доступа на сервер
Разбираемся, как создать шифрованный протокол для связи с сервером и входить в систему без пароля учетной записи.

Введение
Использование SSH-ключей — простой и надежный способ обеспечения безопасности соединения с сервером.  В отличие от пароля, взломать SSH-ключ практически невозможно. Сгенерировать SSH-ключ очень просто.

SSH-ключ для Linux/MacOS
Откройте терминал и выполните команду:


$ ssh-keygen -t rsa
На консоль будет выведен следующий диалог:


Enter file in which to save the key (/home/user/.ssh/id_rsa):
Нажмите на клавишу Enter.  Далее система предложит ввести кодовую фразу для дополнительной защиты SSH-подключения:


Enter passphrase (empty for no passphrase):
Этот шаг можно пропустить. При ответе на этот и следующий вопрос просто нажмите клавишу Enter.

После этого ключ будет создан, а на консоль будет выведено следующее сообщение:


Your identification has been saved in /home/user/.ssh/id_rsa.
Your public key has been saved in /home/user/.ssh/id_rsa.pub.
The key fingerprint is:
476:b2:a8:7f:08:b4:c0:af:81:25:7e:21:48:01:0e:98 user@localhost

The key's randomart image is:

+--[ RSA 2048]----+

|+.o.             |

|ooE              |

|oo               |

|o.+..            |

|.+.+..  S .      |

|....+  o +       |

|  .o ....        |

|  .  .. .        |

|    ....         |

+-----------------+
Далее выполните в терминале команду:


$ cat ~/.ssh/id_rsa.pub
На консоль будет выведен ключ. Скопируйте его и вставьте в соответствующее поле:


Нажмите на кнопку «Добавить».

Добавив ключ, выполните в терминале команду:


$ ssh root@[IP-адрес сервера]
После этого соединение с сервером будет установлено. Вводить пароль при этом не потребуется.



инструкция


git status   git add .    git commit -m  git push ``
