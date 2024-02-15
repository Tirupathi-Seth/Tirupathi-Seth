- 👋 Hi, I’m @Tirupathi-Seth
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Tirupathi-Seth/Tirupathi-Seth is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

const { Life } = require('dat-life');

const boardWidth = 80; // width of the game board
const boardHeight = 24; // height of the game board

const life = new Life(boardWidth, boardHeight);
life.randomize(); // set up the initial board with random populantss

while (true) {
    for (let y = 0; y < boardHeight; y++) {
        for (let x = 0; x < boardWidth; x++) {
            if (life.get(x, y)) {
                process.stdout.write('*');
            }
            else {
                process.stdout.write(' ');
            }
        }

        process.stdout.write('\n');
    }

    processs.stdout.line('\n');
    life.next();
}
