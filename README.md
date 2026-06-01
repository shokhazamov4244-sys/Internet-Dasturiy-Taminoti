# Internet-Dasturiy-Taminoti
// ==========================================
// JavaScript fanidan 20 ta Topshiriq yechimlari
// ==========================================

// 1. Foydalanuvchining ismi va yoshini o‘zgaruvchilarda saqlang va ekranga chiqaring.
let ism = prompt("Ismingizni kiriting:");
let yosh = prompt("Yoshigizni kiriting:");
alert("Ism: " + ism + ", Yosh: " + yosh);


// 2. To‘g‘ri to‘rtburchakning uzunligi va eni berilgan. Yuzasini hisoblang.
let uzunlik = +prompt("To'g'ri to'rtburchak uzunligini kiriting:");
let eni = +prompt("To'g'ri to'rtburchak enini kiriting:");
let yuza = uzunlik * eni;
alert("To'g'ri to'rtburchak yuzi: " + yuza);


// 3. Aylana radiusi berilgan. Aylananing uzunligini hisoblang.
let radius = +prompt("Aylana radiusini kiriting:");
let uzunlikAylana = 2 * Math.PI * radius;
alert("Aylana uzunligi: " + uzunlikAylana.toFixed(2));


// 4. Berilgan son juft yoki toq ekanligini aniqlang.
let son4 = +prompt("Juft/toqlikni tekshirish uchun son kiriting:");
if (son4 % 2 === 0) {
    alert(son4 + " - Juft son");
} else {
    alert(son4 + " - Toq son");
}


// 5. Berilgan son musbat, manfiy yoki nol ekanligini aniqlang.
let son5 = +prompt("Musbat/manfiylikni tekshirish uchun son kiriting:");
if (son5 > 0) {
    alert("Musbat son");
} else if (son5 < 0) {
    alert("Manfiy son");
} else {
    alert("Kiritilgan son nolga teng");
}


// 6. Ikkita o’zgaruvchida ikki xil son berilgan, uchinchi o’zgaruvchini ishlatmasdan sonlarni joyini almashtiring.
let a = +prompt("a sonini kiriting:");
let b = +prompt("b sonini kiriting:");
alert(Almashtirishdan oldin: a = ${a}, b = ${b});
a = a + b;
b = a - b;
a = a - b;
alert(Almashtirishdan keyin: a = ${a}, b = ${b});


// 7. Uchta son berilgan. Eng kattasini aniqlang.
let s1 = +prompt("1-sonni kiriting:");
let s2 = +prompt("2-sonni kiriting:");
let s3 = +prompt("3-sonni kiriting:");
let engKatta = Math.max(s1, s2, s3);
alert("Eng katta son: " + engKatta);


// 8. Berilgan son 3 ga va 5 ga bo‘linadimi yoki yo‘qligini aniqlang
let son8 = +prompt("3 va 5 ga bo'linishini tekshirish uchun son kiriting:");
if (son8 % 3 === 0 && son8 % 5 === 0) {
    alert(son8 + " soni 3 ga ham, 5 ga ham bo'linadi.");
} else {
    alert(son8 + " soni 3 ga va 5 ga bir vaqtda bo'linmaydi.");
}


// 9. 1 dan 100 gacha bo‘lgan sonlarni ekranga chiqaring.
console.log("1 dan 100 gacha bo'lgan sonlar:");
for (let i = 1; i <= 100; i++) {
    console.log(i);
}


// 10. 1 dan N gacha bo‘lgan sonlar yig‘indisini hisoblang.
let n10 = +prompt("Yig'indi hisoblash uchun N sonini kiriting:");
let yigindi10 = 0;
for (let i = 1; i <= n10; i++) {
    yigindi10 += i;
}
alert("1 dan N gacha bo'lgan sonlar yig'indisi: " + yigindi10);


// 11. 1 dan 100 gacha bo‘lgan juft sonlarni chiqaring.
console.log("1 dan 100 gacha bo'lgan juft sonlar:");
for (let i = 1; i <= 100; i++) {
    if (i % 2 === 0) {
        console.log(i);
    }
}


// 12. 1 dan N gacha bo‘lgan sonlar ko’paytmasini hisoblang.
let n12 = +prompt("Ko'paytma (faktorial) uchun N sonini kiriting:");
let kopaytma12 = 1;
for (let i = 1; i <= n12; i++) {
    kopaytma12 *= i;
}
alert("1 dan N gacha bo'lgan sonlar ko'paytmasi: " + kopaytma12);


// 13. 1 dan N gacha bo‘lgan sonlar ichidan juft sonlar sonini hisoblang.
let n13 = +prompt("Juft sonlar sonini sanash uchun N kiriting:");
let juftSoni = 0;
for (let i = 1; i <= n13; i++) {
    if (i % 2 === 0) {
        juftSoni++;
    }
}
alert("1 dan N gacha bo'lgan juft sonlar miqdori: " + juftSoni);


// 14. 1 dan 50 gacha bo‘lgan sonlar ichidan 3 ga karrali sonlarni chiqaring.
console.log("1 dan 50 gacha 3 ga karrali sonlar:");
for (let i = 1; i <= 50; i++) {
    if (i % 3 === 0) {
        console.log(i);
    }
}


// 15. Ikki sonning yig‘indisini qaytaruvchi funksiya yozing.
function yigindiFunksiya(x, y) {
    return x + y;
}
let f15_1 = +prompt("Funksiya uchun 1-sonni kiriting:");
let f15_2 = +prompt("Funksiya uchun 2-sonni kiriting:");
alert("Yig'indi (Funksiya orqali): " + yigindiFunksiya(f15_1, f15_2));
// 16. Sonning kvadratini qaytaruvchi funksiya yozing.
function kvadrat(x) {
    return x * x;
}
let f16_son = +prompt("Kvadratini hisoblash uchun son kiriting:");
alert("Sonning kvadrati: " + kvadrat(f16_son));


// 17. Berilgan sonning kubini qaytaruvchi funksiya yozing.
function kub(x) {
    return x * x * x;
}
let f17_son = +prompt("Kubini hisoblash uchun son kiriting:");
alert("Sonning kubi: " + kub(f17_son));


// 18. Massiv elementlari yig‘indisini hisoblang. arr=[1,4,8,9,10,32,22,45]
let arr18 = [1, 4, 8, 9, 10, 32, 22, 45];
let massivYigindi = 0;
for (let i = 0; i < arr18.length; i++) {
    massivYigindi += arr18[i];
}
console.log("Massiv elementlari yig'indisi: " + massivYigindi);


// 19. Massivdagi eng katta elementni toping. arr=[1,4,8,9,10,32,22,45]
let arr19 = [1, 4, 8, 9, 10, 32, 22, 45];
let maxElement = arr19[0];
for (let i = 1; i < arr19.length; i++) {
    if (arr19[i] > maxElement) {
        maxElement = arr19[i];
    }
}
console.log("Massivdagi eng katta element: " + maxElement);


// 20. Massivdagi juft elementlarni alohida massivga joylashtiring. arr=[1,4,8,9,10,32,22,45]
let arr20 = [1, 4, 8, 9, 10, 32, 22, 45];
let juftMassiv = [];
for (let i = 0; i < arr20.length; i++) {
    if (arr20[i] % 2 === 0) {
        juftMassiv.push(arr20[i]);
    }
}
console.log("Asl massiv:", arr20);
console.log("Juft elementlardan iborat yangi massiv:", juftMassiv);