<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Cute Blog 💕</title>
    <style>
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            background-color: #ffe6f2;
            color: #333;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background-color: #ff99cc;
            color: white;
            padding: 20px;
            border-radius: 10px;
        }
        main {
            margin: 20px auto;
            max-width: 600px;
        }
        .post {
            background: white;
            padding: 15px;
            margin: 10px;
            border-radius: 10px;
            box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
        }
        .post h2 {
            color: #ff4081;
        }
        .post a {
            color: #ff4081;
            text-decoration: none;
            font-weight: bold;
        }
        footer {
            background: #ff99cc;
            color: white;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Cute Blog! 🐰💕</h1>
        <p>Sharing my thoughts, ideas, and cute moments! ✨</p>
    </header>

    <main id="posts-container">
        <!-- Blog posts will be inserted here -->
    </main>

    <footer>
        <p>💖 Made with Love | 2025</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const posts = [
                { title: "🐱 My Cute Cat", content: "My cat is the cutest! She loves to nap all day.", link: "#" },
                { title: "🌸 Aesthetic Room Decor", content: "I decorated my room with pastel colors and fairy lights!", link: "#" },
                { title: "🍰 My Favorite Dessert", content: "I tried baking a strawberry shortcake, and it was delicious!", link: "#" }
            ];

            const postsContainer = document.getElementById("posts-container");

            posts.forEach(post => {
                const postElement = document.createElement("div");
                postElement.classList.add("post");
                postElement.innerHTML = `
                    <h2>${post.title}</h2>
                    <p>${post.content.slice(0, 100)}...</p>
                    <a href="${post.link}">Read More</a>
                `;
                postsContainer.appendChild(postElement);
            });
        });
    </script>
</body>
</html>
