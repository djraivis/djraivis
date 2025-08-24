<p align="center">
  <img src="assets/terminal-animated.svg" alt="Neovim glassy terminal - animated theme switching" width="100%" />
</p>

<!-- Terminal-styled sections: one row, only one can be open at a time -->
<div align="center">
  <table style="width: 100%; table-layout: fixed; border-spacing: 8px;">
    <tr>
      <td style="width: 33.33%; white-space: nowrap;">
        <details id="music-section">
          <summary style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc;">🎵 some music</summary>
          <div align="center" style="margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117;">
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
        </details>
      </td>
      <td style="width: 33.33%; white-space: nowrap;">
        <details id="stats-section">
          <summary style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc;">📊 stats/contributions</summary>
          <div align="center" style="margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117;">
            <img src="https://github-readme-activity-graph.vercel.app/graph?username=djraivis&theme=react-dark&hide_border=true" alt="Contribution Graph" width="100%" />
            <br><br>
            <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=djraivis&theme=transparent" alt="Profile Details" width="48%" />
            <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=djraivis&theme=transparent" alt="Repos per language" width="48%" />
          </div>
        </details>
      </td>
      <td style="width: 33.33%; white-space: nowrap;">
        <details id="home-section">
          <summary style="cursor: pointer; padding: 8px 16px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117; color: #f0f6fc;">🏠 working from home</summary>
          <div align="center" style="margin-top: 20px; padding: 20px; border: 1px solid #30363d; border-radius: 6px; background: #0d1117;">
            <video width="100%" autoplay loop muted playsinline>
              <source src="assets/masthead.mp4" type="video/mp4">
              <source src="assets/masthead.m4v" type="video/mp4">
              Your browser does not support the video tag.
            </video>
          </div>
        </details>
      </td>
    </tr>
  </table>
</div>

<script>
// Only allow one section to be open at a time
document.addEventListener('DOMContentLoaded', function() {
  const details = document.querySelectorAll('details[id$="-section"]');
  
  details.forEach((targetDetail) => {
    targetDetail.addEventListener('click', () => {
      details.forEach((detail) => {
        if (detail !== targetDetail) {
          detail.removeAttribute('open');
        }
      });
    });
  });
});
</script>
