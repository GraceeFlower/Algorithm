//输入一串长度为n的纯大小写字母所需要摁下的最小总键数（分为caps lock和shift 两种方法）
//若需要输入“AAAssA...”这样的只需要在upper函数外部给func穿值并存在常量里即可，此处产生的是“ASxzdASHJ...”这样的字符串
var n = 6;
var str = "";
let func = (type) => String.fromCharCode((Math.random() * 26 + (type).charCodeAt(0)));//65-90 97-122
function product(n) {
    var arrRandom = [];
    for(var i = 0; i < n; i++) {
        arrRandom.push(Math.round(Math.random()) ? func("A") : func("a"));
    }
    str = arrRandom.join("");
    return str;
}
product(n);
console.log(str);

var arr = str.split(/[A-Z]+/).filter((a) => {return a});
var arr1 = str.split(/[a-z]+/).filter((a) => {return a});
var sum = 0;
var tail;
function test(str) {
    var reg =  /[A-Z]{2}$/;
    return tail = reg.test(str);
}
function upper(array) {
    for(var i = 0; i < array.length; i++) {
        if(array[i].length > 1 ) {
            sum = sum + array[i].length + 2;
        }else {
            sum += 2;
        }
    }
    if(tail) {
        sum -= 1;
    }
    return sum;
}
test(str);
upper(arr1);


var low = arr.join('').length;
var result = sum + low;
// console.log(tail);
// console.log(arr);
// console.log(arr1);
console.log(result);
