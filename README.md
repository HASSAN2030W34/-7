// مصفوفة الأسئلة والأجوبة
const questions = [
    // الأسئلة العلمية
    {
        question: "ما هو أكبر كوكب في المجموعة الشمسية؟",
        answer: "المشتري",
        category: "علمية"
    },
    {
        question: "ما هو اسم الغاز الذي نتنفسه؟",
        answer: "الأوكسجين",
        category: "علمية"
    },
    {
        question: "كم عدد كواكب المجموعة الشمسية؟",
        answer: "ثمانية",
        category: "علمية"
    },
    {
        question: "ما هو العنصر الذي يرمز له بالرمز الكيميائي H؟",
        answer: "الهيدروجين",
        category: "علمية"
    },
    {
        question: "ما هي أكبر قارة في العالم من حيث المساحة؟",
        answer: "آسيا",
        category: "علمية"
    },
    {
        question: "ما هو الجزء المسؤول عن نقل الأوكسجين في الدم؟",
        answer: "كريات الدم الحمراء",
        category: "علمية"
    },
    {
        question: "ماذا يسمى عملية تحول الماء من السائل إلى بخار؟",
        answer: "التبخر",
        category: "علمية"
    },
    {
        question: "ما هو أكبر حيوان على وجه الأرض؟",
        answer: "الحوت الأزرق",
        category: "علمية"
    },
    {
        question: "ما هي وحدة قياس الطول في النظام المتري؟",
        answer: "المتر",
        category: "علمية"
    },
    {
        question: "أي من الحيوانات التالية لا يبيض: الأفعى، السمكة، الأرنب؟",
        answer: "الأرنب",
        category: "علمية"
    },

    // الأسئلة التاريخية
    {
        question: "من هو أول رئيس للمملكة العربية السعودية؟",
        answer: "الملك عبد العزيز آل سعود",
        category: "تاريخية"
    },
    {
        question: "ما هي السنة التي تأسست فيها المملكة العربية السعودية؟",
        answer: "1932",
        category: "تاريخية"
    },
    {
        question: "من هو القائد الذي فاز في معركة مؤتة؟",
        answer: "زيد بن حارثة",
        category: "تاريخية"
    },
    {
        question: "ما هو اسم أول مسجد بني في الإسلام؟",
        answer: "مسجد قباء",
        category: "تاريخية"
    },
    {
        question: "في أي سنة تم بناء برج المملكة في الرياض؟",
        answer: "1999",
        category: "تاريخية"
    },
    {
        question: "من هو الخليفة العباسي الذي أسس بغداد؟",
        answer: "الخليفة المنصور",
        category: "تاريخية"
    },
    {
        question: "ما هو اسم العاصمة الإسلامية في فترة الخلافة الأمويّة؟",
        answer: "دمشق",
        category: "تاريخية"
    },

    // الأسئلة الجغرافية
    {
        question: "ما هي أكبر صحراء في العالم؟",
        answer: "الصحراء الكبرى",
        category: "جغرافية"
    },
    {
        question: "ما هو أطول نهر في العالم؟",
        answer: "نهر النيل",
        category: "جغرافية"
    },
    {
        question: "ما هي العاصمة السعودية؟",
        answer: "الرياض",
        category: "جغرافية"
    },
    {
        question: "في أي قارة يقع جبل إيفرست؟",
        answer: "آسيا",
        category: "جغرافية"
    },
    {
        question: "ما هي الدولة التي تعتبر أكبر دولة في العالم من حيث المساحة؟",
        answer: "روسيا",
        category: "جغرافية"
    },
    {
        question: "أين تقع مدينة الأهرامات الشهيرة؟",
        answer: "في مصر",
        category: "جغرافية"
    },

    // الألغاز
    {
        question: "ما هو الشيء الذي يملك أوراقًا ولكن لا يعيش؟",
        answer: "الكتاب",
        category: "ألغاز"
    },
    {
        question: "ما هو الشيء الذي يزداد كلما أخذت منه؟",
        answer: "الحفرة",
        category: "ألغاز"
    },
    {
        question: "ما هو الشيء الذي لا يمشي إلا بالضرب؟",
        answer: "المطرقة",
        category: "ألغاز"
    },
    {
        question: "شيء في السماء لا يمكن رؤيته إلا عندما يكون على الأرض. ما هو؟",
        answer: "قوس قزح",
        category: "ألغاز"
    },
    {
        question: "ما هو الشيء الذي يجري بلا ماء؟",
        answer: "الساعة",
        category: "ألغاز"
    },
    {
        question: "أين يمكن للغريق أن يغرق أكثر من مرة في نفس المكان؟",
        answer: "في البحر",
        category: "ألغاز"
    },
    {
        question: "أين يمكنك أن تجد الشمس في الليل؟",
        answer: "في الحلم",
        category: "ألغاز"
    },
    {
        question: "ما هو الشيء الذي يمكن أن يحمل أطنانًا من الأشياء لكنه لا يزن شيئًا؟",
        answer: "الظل",
        category: "ألغاز"
    },
    {
        question: "شيء يسير بلا قدمين ولا يطير، ولكنه لا يتوقف. ما هو؟",
        answer: "الزمن",
        category: "ألغاز"
    },
    {
        question: "ما هو الشيء الذي لا يتكلم ولكن إذا جاع يصرخ؟",
        answer: "الجرس",
        category: "ألغاز"
    }
];

// دالة لاختيار سؤال عشوائي
function getRandomQuestion() {
    const randomIndex = Math.floor(Math.random() * questions.length);
    const question = questions[randomIndex];
    return question;
}

// عرض السؤال في الصفحة
function displayQuestion() {
    const question = getRandomQuestion();
    document.getElementById("question").textContent = question.question;
    document.getElementById("answer").value = "";
    document.getElementById("result").textContent = "";
    return question;
}

// التحقق من الإجابة
function checkAnswer() {
    const userAnswer = document.getElementById("answer").value.trim().toLowerCase();
    const currentQuestion = document.getElementById("question").textContent;
    const correctAnswer = questions.find(q => q.question === currentQuestion).answer.toLowerCase();
    const result = document.getElementById("result");

    if (userAnswer === correctAnswer) {
        result.textContent = "إجابة صحيحة!";
        result.style.color = "green";
    } else {
        result.textContent = "إجابة خاطئة! حاول مرة أخرى.";
        result.style.color = "red";
    }
}

// بداية اللعبة
displayQuestion();
