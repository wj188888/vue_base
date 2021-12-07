break表示立即终止循环，他只能用在循环语句中，在for循环和while循环中都可以使用；
for (var i =0; i< 10; i++) {
    console.log(i);
    if (i == 4) {
        break;
    }
}