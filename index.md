---
title: "Lihi Bolokan — Personal Page"
---

<style>
  :root {
    --bg: #ffffff;
    --text: #111111;
    --muted: #666666;
    --link: #0a66c2;
    --card: #f6f6f6;
  }
  @media (prefers-color-scheme: dark) {
    :root {
      --bg: #0f1115;
      --text: #e9eef5;
      --muted: #9aa4b2;
      --link: #68a8ff;
      --card: #151821;
    }
  }
  html, body {
    padding: 0; margin: 0; background: var(--bg); color: var(--text);
    font: 16px/1.6 -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
  }
  .wrap {
    max-width: 980px; padding: 40px 20px; margin: 0 auto;
  }
  .card {
    background: var(--card);
    border-radius: 18px;
    box-shadow: 0 8px 24px rgba(0,0,0,.08);
    padding: 28px;
  }
  .grid {
    display: grid;
    grid-template-columns: 340px 1fr;
    gap: 28px;
    align-items: center;
  }
  .photo {
    width: 100%; border-radius: 14px; display: block;
    object-fit: cover; aspect-ratio: 4 / 5;
  }
  h1 {
    margin: 0 0 10px 0; font-size: 28px; letter-spacing: .2px;
  }
  p { margin: 0 0 14px 0; }
  .muted { color: var(--muted); }
  a { color: var(--link); text-decoration: none; }
  a:hover { text-decoration: underline; }
  ul { margin: 10px 0 0 20px; }
  .footer { margin-top: 16px; font-size: 14px; color: var(--muted); }
  @media (max-width: 780px) {
    .grid { grid-template-columns: 1fr; }
  }
</style>

<div class="wrap">
  <div class="card">
    <div class="grid">
      <!-- LEFT: biology-related image -->
      <img class="photo" src="assets/biology.jpg" alt="Biology-themed image">

      <!-- RIGHT: content -->
      <div>
        <h1>Welcome to my personal page!</h1>
        <p>
          I’m an <strong>M.Sc. student</strong> at the <strong>Weizmann Institute of Science</strong>,
          currently doing a rotation in <strong>Prof. Eldad Tzahor’s</strong> lab, which focuses on
          regenerative medicine with particular relevance to adult heart disease.
          Lab webpage:
          <a href="https://www.weizmann.ac.il/mcb/tzahor/" target="_blank" rel="noopener">Tzahor Lab</a>.
        </p>

        <p>
          I completed my <strong>B.Sc.</strong> in <strong>Biology, Psychology, and Neuroscience</strong>
          at <strong>Tel Aviv University</strong>.
        </p>

        <p>
          Outside the lab, I like to travel, read, cook, and enjoy meals with friends.
        </p>

        <h3>Connect</h3>
        <p>
          If my work interests you or if you have any questions, feel free to reach out:
          <a href="mailto:lihi.bolokan@weizmann.ac.il">lihi.bolokan@weizmann.ac.il</a>
        </p>

        <p class="footer">
          © <span id="y"></span> Lihi Bolokan
        </p>
        <script>
          document.getElementById('y').textContent = new Date().getFullYear();
        </script>
      </div>
    </div>
  </div>
</div>
