// --- 3-in-1 Game Pack ---

console.log("--- Welcome to Multi-Game Hub! ---");

// 1. Number Guessing Game Logic
function guessNumber(playerInput) {
    let luckyNumber = Math.floor(Math.random() * 10) + 1;
    if(playerInput == luckyNumber) {
        return "Mubarak ho! Aap jeet gaye. Lucky number " + luckyNumber + " hi tha.";
    } else {
        return "Afsoos! Sahi number " + luckyNumber + " tha. Dobara koshish karein.";
    }
}

// 2. Simple Chat Bot
function chatWithBot(msg) {
    if(msg.includes("hello")) return "Hello! Kaise hain aap?";
    if(msg.includes("game")) return "Aap Number Guessing ya Emoji game khel sakte hain.";
    return "Main abhi seekh raha hoon!";
}

// 3. Game Runner
console.log("Game 1 Result: " + guessNumber(5)); // Misal ke taur par 5 check kiya
console.log("Bot Response: " + chatWithBot("hello"));

console.log("--- Game is Ready to Play! ---");
