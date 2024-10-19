<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Encouragement for Raeanne</title>
    <style>
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #fdf5e6;
            border: 10px solid #ffc0cb;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }
        #clickButton {
            background-color: #ff69b4;
            color: white;
            border: none;
            padding: 30px;
            font-size: 20px;
            cursor: pointer;
            border-radius: 30px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            max-width: 80%;
            white-space: normal;
        }
        #clickButton:active {
            background-color: #ff1493;
            transform: scale(0.95);
        }
    </style>
</head>
<body>
    <button id="clickButton">Click Me!</button>

    <script>
        // Create a list of 200 encouraging phrases for Raeanne "Rae"
        const phrases = [
            "Raeanne, you are unstoppable! Keep shining!",
            "Your hustle at Sportys and Sliders is unmatched! Keep kicking ass!",
            "Your customers absolutely love you because you bring so much joy to everyone around you! Keep it up!",
            "You have an amazing family that supports you. You are making them so proud!",
            "You are a powerhouse! Working two jobs and still managing it all, you are incredible!",
            "Your dedication to Raise A Glass Event Bartending is truly inspiring. You are building something amazing!",
            "Keep working out and stay consistent. It's great for your mind and your soul!",
            "You are a beacon of positivity. Keep spreading those positive vibes!",
            "Rae Rae, your energy behind the bar makes everyone's day brighter. Keep being the light!",
            "Artie and Brooklyn are lucky to have you. You take such great care of them!",
            "You are stronger than any challenge that comes your way. Keep pushing through!",
            "You are resilient, and every day you are getting better! Keep moving forward!",
            "Every drink you mix is a masterpiece. You are a true artist behind the bar!",
            "Staying consistent with your health and workouts will help keep your amazing spirit even stronger!",
            "Remember that your smile makes everyone's day. Keep smiling and spreading joy!",
            "Your customers love you for your energy, and Austin loves you for everything you are. Keep being amazing!",
            "Brooklyn's elegance and Artie's craziness make for a perfect pair—just like you and Austin!",
            "Never underestimate your power to make a difference in someone's life. You do it every day!",
            "You are loved beyond words. Your kindness makes the world better!",
            "Your dedication to bartending, family, and health is inspiring. You are unstoppable!",
            "Every day is another chance to be the best version of yourself. Keep going!",
            "You have the ability to make everyone feel at home—just like Artie and Brooklyn do when you're around!",
            "Your positive attitude lights up even the darkest rooms. Keep shining bright!",
            "Your passion for what you do makes you stand out. Keep hustling, girl!",
            "Staying healthy is a journey, and you're doing an incredible job. Keep at it!",
            "You're building something great with Raise A Glass Event Bartending. Keep crushing it!",
            "Every step forward counts. You are doing an amazing job!",
            "Your workouts are not just for your body but also for your mind. Keep that positive momentum!",
            "You are an incredible girlfriend, and Austin is lucky to have you. Keep being yourself!",
            "Your strength shows in everything you do. Keep showing up for yourself!",
            "Every day is a new opportunity, and you make the most of it. Keep hustling!",
            "Keep believing in yourself. The world is better because of you!",
            "The love you have for your family shines through everything you do. Keep being wonderful!",
            "The way you handle your work at both bars is truly inspiring. You make it look easy!",
            "You are creating memories every day that will last forever. Keep being amazing!",
            "Artie may be nuts, but he adores you, and Brooklyn looks up to you too. You are their hero!",
            "You are making a difference at Sportys, Sliders, and beyond. Keep shining!",
            "Working out isn't just physical—it's strengthening your incredible spirit too. Keep going!",
            "Your love for your family is one of your greatest strengths. Keep spreading that love!",
            "Austin is always cheering for you. You are never alone in your journey!",
            "Every click you make is a step towards positivity and self-improvement. You got this!",
            "Bartending is your art, and every drink tells a story. Keep painting those masterpieces!",
            "Your ability to connect with people is a true gift. Keep making others feel special!",
            "You have all the strength you need to succeed. Keep moving forward, step by step!",
            "Your energy is infectious. Never stop sharing it with the world!",
            "Remember, consistency is key. You are building something beautiful with your hard work!",
            "You are a true hustler, and your dedication inspires everyone around you. Keep at it!",
            "You are making a positive impact everywhere you go. Keep spreading good vibes!",
            "Brooklyn's elegance reminds you to stay graceful. You are beautiful inside and out!",
            "Your journey to stay healthy is admirable. Keep going, and remember it's for your mind too!",
            "Austin loves seeing you grow. Keep being the best version of yourself!",
            "You are strong, beautiful, and capable of anything you put your mind to!",
            "Every day at Sportys and Sliders, you make a difference in someone's life. Keep being you!",
            "You are resilient and always find a way to make things work. Keep pushing forward!",
            "Your journey to becoming debt-free is so inspiring. Imagine the freedom—you're getting there!",
            "Rae, $10,000 in the bank is just around the corner. Keep saving, you're almost there!",
            "Your dedication to reaching $20,000 saved is amazing! You are unstoppable on your financial journey!",
            "Imagine the day you buy your first house. You're making it happen, step by step! Keep believing!",
            "Your goals are huge, and your effort matches them. You are capable of so much, Rae!",
            "Every hustle brings you closer to your dreams. Keep up the amazing work!",
            "You are creating the future you want—keep going and don't look back!",
            "Saving money is tough, but you are tougher! That $10,000 goal is within reach!",
            "Raeanne, you are building something truly special. Keep the faith and keep hustling!",
            "Imagine walking into your very own home. You deserve it, and you're working so hard to get there!",
            "Rae Rae, every penny you save, every job you take, it's all leading you to greatness!",
            "Financial freedom is coming, Rae. Keep doing what you're doing, and you'll get there!",
            "Debt-free life is closer every day. Keep pushing forward, you're doing incredible!",
            "Saving up $20,000 might seem like a mountain, but you're climbing it! Step by step!",
            "The dedication you have towards your financial goals is inspiring. Keep going, Rae Rae!",
            "Imagine how proud you will feel when you buy your first home. You are on your way!",
            "Austin is right by your side, cheering you on every step of the way! You are never alone!",
            "You are making sacrifices now to enjoy a brighter future. Keep it up! You are amazing!",
            "Your strength is in your discipline, Rae. Keep working on those goals, you're almost there!",
            "The road to being debt-free is not easy, but you are tougher than anything that comes your way!",
            "Imagine that $20,000 in the bank and what it means for you. You're doing incredible!",
            "You're saving for a life you love, and you are making it happen. Every step counts!",
            "Rae, your efforts will lead to financial freedom. You're almost at the finish line—keep at it!",
            "The future you envision is coming true, one day at a time. Stay consistent and keep shining!",
            "Every goal you set, you are conquering it. Debt-free, house, savings—you're achieving it all!",
            "You inspire those around you, including Austin, with your determination. Keep going, Rae!",
            "Remember, all this hard work is for your freedom and happiness. You're almost there!",
            "You are going to achieve your financial dreams, and no one deserves it more than you, Rae!",
            "Picture your life debt-free and in your own house—it's closer than you think. Keep hustling!",
            "Austin believes in you, and so do all your loved ones. Keep going, you are unstoppable!",
            "You are working so hard, and it will pay off. Keep saving, working, and believing in yourself!",
            "Debt-free, $20,000 saved, first house—these are all things you're making happen. Keep at it, Rae!",
            "The future is bright, Raeanne. Your discipline and hard work are taking you far!",
            "Imagine hosting family and friends in your own home. It's coming—keep pushing towards it!",
            "Your journey is inspiring. Keep saving, keep working, and keep being amazing!",
            "Every day you get closer to financial freedom. You are capable of incredible things!",
            "The dream of owning your own home is coming true because you are making it happen!",
            "Your hustle is unmatched, Rae. Keep shining and making those dreams come true!",
            "Austin is your biggest supporter, and he knows you're capable of amazing things. Keep going!",
            "Your future is bright, your goals are in reach, and you are unstoppable! Keep working hard!",
            "Imagine yourself debt-free, in your own home, living the life you want. You are almost there!",
            "The dedication you show every day is leading you to greatness!",
            "Raeanne, every ounce of effort you put in is bringing you closer to your dreams!",
            "You make the impossible seem achievable. Keep striving and reaching new heights!",
            "Your commitment to your dreams is inspiring to everyone around you. Keep it going!",
            "Rae Rae, every little sacrifice is adding up to big rewards. Keep the end in mind!",
            "The love and kindness you give to others is returned to you tenfold. Keep being amazing!",
            "You're making decisions that are setting up your future. Keep going and stay focused!",
            "Austin knows how strong you are, and so do you. Keep pushing through any obstacles!",
            "With every click, every job, every hustle, you're moving toward something extraordinary!",
            "You have a vision for your life, and you're making it real one day at a time. Keep at it!",
            "Saving and budgeting aren't always easy, but you're absolutely crushing it! Keep it up!",
            "Imagine how incredible it'll be when you reach your financial goals—you're so close!",
            "Austin sees your hard work and determination, and it inspires him every single day!",
            "You are strong, capable, and deserving of all the wonderful things you're working towards!",
            "Keep in mind, Rae, that every small step leads to giant leaps in your future!",
            "Raeanne, you've got this! You're closer to freedom and happiness than ever before!",
            "When you save, you’re not just saving money—you’re saving dreams! Keep it up, Rae!",
            "The joy you'll feel when you're debt-free is going to be immeasurable. Keep pushing forward!",
            "The strength you are showing now is building a future full of endless possibilities!",
            "Austin believes in you completely, and your hard work is going to bring so much good!",
            "You've got everything it takes to build the life you desire. Keep striving for greatness!",
            "Picture your beautiful house and what it means for your journey. It’s going to be amazing!",
            "Your determination is incredible. Keep saving, keep striving, and stay on track!",
            "Debt-free means more freedom for adventures and joy. You’re getting there, Rae!",
            "Austin knows you'll get there, and you know it too. Keep the faith and keep hustling!",
            "You're setting an amazing example for everyone around you. Keep up the fantastic work!"
        ];

        let clickButton = document.getElementById('clickButton');
        
        // Add click event listener to the button
        clickButton.addEventListener('click', () => {
            // Choose a random phrase each time Rae clicks
            const randomIndex = Math.floor(Math.random() * phrases.length);
            clickButton.innerText = phrases[randomIndex];

            // Make the button move to a random position on the screen
            clickButton.style.position = 'absolute';
            clickButton.style.top = Math.random() * (window.innerHeight - clickButton.offsetHeight) + 'px';
            clickButton.style.left = Math.random() * (window.innerWidth - clickButton.offsetWidth) + 'px';

            // Change button color randomly for a fun effect
            const colors = ['#ff69b4', '#ff1493', '#ff6ec7', '#ff85a1', '#ffa07a', '#ffb6c1', '#ff6347', '#ff4500', '#ff8c00', '#ffdab9'];
            clickButton.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
        });
    </script>
</body>
</html>
