# 2-2-1
Video and picture ai generator 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Flame Creative Studio — AI-powered video & image creator with stunning visuals." />
  <title>Flame Creative Studio - Advanced Video &amp; Image Creator</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Outfit:wght@600;700&display=swap');
    /* [YOUR EXISTING CSS HERE] */
  </style>
</head>
<body>
  <!-- Starfield Background -->
  <div id="starfield" aria-hidden="true"></div>

  <!-- Header -->
  <header>
    <div class="container" role="banner">
      <div class="logo" tabindex="0" aria-label="Flame Creative Studio Logo">flame²⁺²=1</div>
      <nav aria-label="Primary Navigation">
        <ul>
          <li><a href="#create" class="hidden-on-login">Create</a></li>
          <li><a href="#about" class="hidden-on-login">About Me</a></li>
          <li>
            <button id="login-btn" class="hidden-on-login">Log In</button>
            <button id="logout-btn" class="hidden-on-logout" style="display:none;">Log Out</button>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Extraordinary Video &amp; Image Creator</h1>
    <p>Create stunning videos and images with ease. Choose style, voices, and length — then download your masterpiece.</p>
    <button class="btn-cta hidden-on-login" id="hero-login-btn">Log In to Start Creating</button>
  </section>

  <main tabindex="-1">
    <!-- Create Section -->
    <section id="create" class="card">
      <h2>Create Your Video or Picture</h2>
      <form id="create-form" autocomplete="off">
        <label for="description">Description</label>
        <textarea id="description" name="description" placeholder="Enter your description…" required rows="6"></textarea>

        <fieldset>
          <legend>Choose Style</legend>
          <div class="radio-group">
            <input type="radio" id="style-animated" name="style" value="animated" required />
            <label for="style-animated">Animated</label>
            <input type="radio" id="style-realistic" name="style" value="realistic" />
            <label for="style-realistic">Realistic</label>
            <input type="radio" id="style-dreamy" name="style" value="dreamy" />
            <label for="style-dreamy">Dreamy</label>
            <input type="radio" id="style-bw" name="style" value="black_and_white" />
            <label for="style-bw">Black &amp; White</label>
          </div>
        </fieldset>

        <label for="video-length">Video Length (seconds)</label>
        <select id="video-length" name="video-length" required>
          <option value="5">5</option>
          <option value="10" selected>10</option>
          <option value="15">15</option>
          <option value="30">30</option>
          <option value="60">60</option>
        </select>

        <label for="voice">Choose Character Voice</label>
        <select id="voice" name="voice" required>
          <optgroup label="Female Voices">
            <option value="female_1">Female 1</option>
            <option value="female_2">Female 2</option>
            <option value="female_3">Female 3</option>
            <option value="female_4">Female 4</option>
          </optgroup>
          <optgroup label="Male Voices">
            <option value="male_1">Male 1</option>
            <option value="male_2">Male 2</option>
            <option value="male_3">Male 3</option>
            <option value="male_4">Male 4</option>
          </optgroup>
        </select>

        <fieldset>
          <legend>Select Speech Type</legend>
          <input type="radio" id="dialogue" name="speech" value="dialogue" required />
          <label for="dialogue">Dialogue</label>
          <input type="radio" id="monologue" name="speech" value="monologue" />
          <label for="monologue">Monologue</label>
        </fieldset>

        <button type="submit" class="btn-create">Create Video/Picture</button>
      </form>

      <div id="result-container">
        <div id="result-preview"><span>No content created yet.</span></div>
        <button id="download-button">Download</button>
      </div>
    </section>

    <!-- About Section -->
    <section id="about">
      <h2>About Me</h2>
      <p>My name is <strong>Goshan</strong>. I am studying at the University of Halabja, majoring in English.</p>
      <p>My Facebook: <a href="https://www.facebook.com/goshan.mzafar" target="_blank" rel="noopener noreferrer">goshan.mzafar</a></p>
      <p>For feedback and suggestions, feel free to message me.</p>
    </section>
  </main>

  <!-- Login Modal (truncated for brevity) -->
  <div id="login-modal" class="hidden"> ... </div>
</body>
</html>
