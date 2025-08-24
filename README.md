<p align="center">
  <img src="assets/terminal-animated.svg" alt="Neovim glassy terminal - animated theme switching" width="100%" />
</p>

<!-- Terminal-styled sections: buttons in one row, content spans full width -->
<div align="center">
  <!-- Button row -->
  <table style="width: 100%; table-layout: fixed; border-spacing: 8px;">
    <tr>
      <td style="width: 33.33%; white-space: nowrap;">
        <button onclick="toggleSection('music')" id="music-btn" style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc; width: 100%;">🎵 some music</button>
      </td>
      <td style="width: 33.33%; white-space: nowrap;">
        <button onclick="toggleSection('stats')" id="stats-btn" style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc; width: 100%;">📊 stats/contributions</button>
      </td>
      <td style="width: 33.33%; white-space: nowrap;">
        <button onclick="toggleSection('home')" id="home-btn" style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc; width: 100%;">🏠 working from home</button>
      </td>
    </tr>
  </table>
</div>

<!-- Full-width content sections -->
<div id="music-content" style="display: none; margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; width: 100%;" align="center">
  <a href="https://www.youtube.com/watch?v=CTM15wqVDFE" target="_blank">
    <img src="https://img.youtube.com/vi/CTM15wqVDFE/hqdefault.jpg" width="200" alt="YouTube video" />
  </a>
  <a href="https://www.youtube.com/watch?v=XiAr1wk68WQ" target="_blank">
    <img src="https://img.youtube.com/vi/XiAr1wk68WQ/hqdefault.jpg" width="200" alt="YouTube video" />
  </a>
  <a href="https://www.youtube.com/watch?v=B7uOajUwG-U" target="_blank">
    <img src="https://img.youtube.com/vi/B7uOajUwG-U/hqdefault.jpg" width="200" alt="YouTube video" />
  </a>
  <a href="https://www.youtube.com/watch?v=-ppRBqNxr-E" target="_blank">
    <img src="https://img.youtube.com/vi/-ppRBqNxr-E/hqdefault.jpg" width="200" alt="YouTube video" />
  </a>
</div>

<div id="stats-content" style="display: none; margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; width: 100%;" align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=djraivis&theme=react-dark&hide_border=true" alt="Contribution Graph" width="100%" />
  <br><br>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=djraivis&theme=transparent" alt="Profile Details" width="48%" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=djraivis&theme=transparent" alt="Repos per language" width="48%" />
</div>

<div id="home-content" style="display: none; margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; width: 100%;" align="center">
  <video width="100%" autoplay loop muted playsinline>
    <source src="assets/masthead.mp4" type="video/mp4">
    <source src="assets/masthead.m4v" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<script>
function toggleSection(section) {
  // Hide all content sections
  const sections = ['music', 'stats', 'home'];
  sections.forEach(s => {
    const content = document.getElementById(s + '-content');
    const btn = document.getElementById(s + '-btn');
    if (s === section) {
      // Toggle the clicked section
      if (content.style.display === 'none' || !content.style.display) {
        content.style.display = 'block';
        btn.style.background = '#21262d';
      } else {
        content.style.display = 'none';
        btn.style.background = '#0d1117';
      }
    } else {
      // Hide other sections
      content.style.display = 'none';
      btn.style.background = '#0d1117';
    }
  });
}
</script>
