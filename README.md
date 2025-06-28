# Vibenet
My custom social media platform
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>VibeNet</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #0f0f0f;
      color: #fff;
      padding: 20px;
    }
    header {
      background: #1a1a1a;
      padding: 15px;
      text-align: center;
      font-size: 2em;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-bottom: 30px;
    }
    nav a {
      text-decoration: none;
      color: #fff;
      background: #333;
      padding: 10px 20px;
      border-radius: 8px;
      transition: 0.3s;
    }
    nav a:hover {
      background: #4b4bff;
    }
    .profile {
      max-width: 500px;
      background: #1a1a1a;
      margin: auto;
      padding: 20px;
      border-radius: 10px;
      text-align: center;
    }
    .profile img {
      width: 120px;
      border-radius: 50%;
      border: 3px solid #4b4bff;
    }
    .profile h2 {
      margin-top: 15px;
    }
    .post-box {
      margin-top: 30px;
      background: #1a1a1a;
      padding: 15px;
      border-radius: 10px;
    }
    textarea {
      width: 100%;
      height: 80px;
      padding: 10px;
      border-radius: 8px;
      border: none;
      resize: none;
      font-size: 1em;
      background: #222;
      color: #fff;
    }
    button {
      margin-top: 10px;
      padding: 10px 15px;
      background: #4b4bff;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    .post {
      background: #2c2c2c;
      margin-top: 20px;
      padding: 15px;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header>VibeNet</header>

  <nav>
    <a href="#">Home</a>
    <a href="#">Explore</a>
    <a href="#">Profile</a>
    <a href="#">Settings</a>
  </nav>

  <div class="profile">
    <img src="https://i.imgur.com/Zi6v09M.png" alt="Profile Picture" />
    <h2>Sadim</h2>
    <p>Founder of VibeNet 🧠</p>
  </div>

  <div class="post-box">
    <h3>What's on your mind?</h3>
    <textarea id="userPost" placeholder="Type something..."></textarea>
    <button onclick="postNow()">Post</button>
  </div>

  <div id="postArea"></div>

  <script>
    function postNow() {
      const postText = document.getElementById('userPost').value;
      if (postText.trim() !== "") {
        const postDiv = document.createElement('div');
        postDiv.className = 'post';
        postDiv.innerText = postText;
        document.getElementById('postArea').prepend(postDiv);
        document.getElementById('userPost').value = "";
      }
    }
  </script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>VibeNet</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #0f0f0f;
      color: #fff;
      padding: 20px;
    }
    header {
      background: #1a1a1a;
      padding: 15px;
      text-align: center;
      font-size: 2em;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-bottom: 30px;
    }
    nav a {
      text-decoration: none;
      color: #fff;
      background: #333;
      padding: 10px 20px;
      border-radius: 8px;
      transition: 0.3s;
    }
    nav a:hover {
      background: #4b4bff;
    }
    .profile {
      max-width: 500px;
      background: #1a1a1a;
      margin: auto;
      padding: 20px;
      border-radius: 10px;
      text-align: center;
    }
    .profile img {
      width: 120px;
      border-radius: 50%;
      border: 3px solid #4b4bff;
    }
    .profile h2 {
      margin-top: 15px;
    }
    .post-box {
      margin-top: 30px;
      background: #1a1a1a;
      padding: 15px;
      border-radius: 10px;
    }
    textarea {
      width: 100%;
      height: 80px;
      padding: 10px;
      border-radius: 8px;
      border: none;
      resize: none;
      font-size: 1em;
      background: #222;
      color: #fff;
    }
    button {
      margin-top: 10px;
      padding: 10px 15px;
      background: #4b4bff;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    .post {
      background: #2c2c2c;
      margin-top: 20px;
      padding: 15px;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header>VibeNet</header>

  <nav>
    <a href="#">Home</a>
    <a href="#">Explore</a>
    <a href="#">Profile</a>
    <a href="#">Settings</a>
  </nav>

  <div class="profile">
    <img src="https://i.imgur.com/Zi6v09M.png" alt="Profile Picture" />
    <h2>Sadim</h2>
    <p>Founder of VibeNet 🧠</p>
  </div>

  <div class="post-box">
    <h3>What's on your mind?</h3>
    <textarea id="userPost" placeholder="Type something..."></textarea>
    <button onclick="postNow()">Post</button>
  </div>

  <div id="postArea"></div>

  <script>
    function postNow() {
      const postText = document.getElementById('userPost').value;
      if (postText.trim() !== "") {
        const postDiv = document.createElement('div');
        postDiv.className = 'post';
        postDiv.innerText = postText;
        document.getElementById('postArea').prepend(postDiv);
        document.getElementById('userPost').value = "";
      }
    }
  </script>

</body>
</html>
<script>
  function postNow() {
    const postText = document.getElementById('userPost').value;
    if (postText.trim() !== "") {
      const postDiv = document.createElement('div');
      postDiv.className = 'post';
      postDiv.innerHTML = `
        <p>${postText}</p>
        <button class="likeBtn" onclick="likePost(this)">❤️ Like <span>0</span></button>
        <div class="comments"></div>
        <input class="commentInput" type="text" placeholder="Write a comment..." onkeypress="handleComment(event, this)">
      `;
      document.getElementById('postArea').prepend(postDiv);
      document.getElementById('userPost').value = "";
    }
  }

  function likePost(button) {
    let countSpan = button.querySelector('span');
    let count = parseInt(countSpan.innerText);
    countSpan.innerText = count + 1;
  }

  function handleComment(e, input) {
    if (e.key === "Enter" && input.value.trim() !== "") {
      const commentBox = input.previousElementSibling;
      const comment = document.createElement("p");
      comment.style.marginTop = "5px";
      comment.style.fontSize = "0.9em";
      comment.innerText = `💬 ${input.value}`;
      commentBox.appendChild(comment);
      input.value = "";
    }
  }
</script>
<div class="sidebar">
  <h3>Suggested to Follow</h3>
  <div class="user-suggestion">
    <img src="https://i.pravatar.cc/50?img=3" alt="User1" />
    <div>
      <p><strong>Rafiq</strong></p>
      <button onclick="toggleFollow(this)">Follow</button>
    </div>
  </div>
  <div class="user-suggestion">
    <img src="https://i.pravatar.cc/50?img=5" alt="User2" />
    <div>
      <p><strong>Jannat</strong></p>
      <button onclick="toggleFollow(this)">Follow</button>
    </div>
  </div>
  <div class="user-suggestion">
    <img src="https://i.pravatar.cc/50?img=7" alt="User3" />
    <div>
      <p><strong>Arif</strong></p>
      <button onclick="toggleFollow(this)">Follow</button>
    </div>
  </div>
</div>
.sidebar {
  position: fixed;
  right: 10px;
  top: 100px;
  width: 250px;
  background: #1a1a1a;
  padding: 15px;
  border-radius: 10px;
  color: #ddd;
  font-size: 0.9em;
  max-height: 70vh;
  overflow-y: auto;
}

.user-suggestion {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.user-suggestion img {
  border-radius: 50%;
  width: 50px;
  margin-right: 10px;
  border: 2px solid #4b4bff;
}

.user-suggestion button {
  background: #4b4bff;
  border: none;
  color: white;
  padding: 5px 12px;
  border-radius: 6px;
  cursor: pointer;
  font-size: 0.8em;
}

.user-suggestion button.following {
  background: #777;
}
function toggleFollow(btn) {
  if (btn.classList.contains('following')) {
    btn.classList.remove('following');
    btn.innerText = 'Follow';
  } else {
    btn.classList.add('following');
    btn.innerText = 'Following';
  }
}
