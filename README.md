<div align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=500&size=24&pause=1000&color=00FF00&center=true&vCenter=true&width=600&lines=SYSTEM+TERMINAL+INITIALIZED...;AUTHENTICATION+COMPLETE...;WELCOME,+OPERATIVE+AGRA.;ACCESSING+MAINFRAME..." alt="Typing SVG" />
  </a>
</div>

<br>

<div align="center">
  <table border="0" style="border-collapse: separate; border-spacing: 0; background-color: #050505; border-left: 4px solid #00F0FF; border-right: 4px solid #FF003C; color: #A9B2C3;" width="85%">
    <tr>
      <td align="center" width="30%" style="padding: 15px; border-top: 1px solid #00F0FF; border-bottom: 1px solid #00F0FF;">
        <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExMjM4YjVkNzE0NTg3MjRjNzM1MTE0Y2QwYjZjYjZjYjZjYjZjYjZjYjZjYjZjYjZjYjZjYjZq/26tn33aiTi1jSqZ4Q/giphy.gif" width="180" alt="Blue Hologram Anatomy"><br><br><code style="color: #00F0FF;">> BIO_SCAN_PASS</code>
      </td>
      <td width="70%" style="padding: 20px; border-top: 1px solid #FF003C; border-bottom: 1px solid #FF003C; text-align: left;">
        <h2 style="color: #FF003C; margin-top: 0;">[ DOSSIER: AGRA ]</h2>
        <ul style="list-style-type: none; padding-left: 0; line-height: 1.8;">
          <li><strong style="color: #00F0FF;">ROLE:</strong> Frontend Architect & Interface Engineer</li>
          <li><strong style="color: #00F0FF;">CORE_SYSTEMS:</strong> React.js, Next.js, Tailwind CSS</li>
          <li><strong style="color: #00F0FF;">VISUAL_PROTOCOL:</strong> Minimalist Agency Emblems & Geometric Vectors</li>
          <li><strong style="color: #00F0FF;">NEURAL_NETWORK:</strong> AI Image Generation & Iterative Prompting</li>
          <li><strong style="color: #00F0FF;">TELEMETRY:</strong> GT World Challenge, Le Mans, Endurance Mechanics</li>
        </ul>
        <hr style="border: 0; border-bottom: 1px dashed #FF003C;">
      </td>
    </tr>
  </table>
</div>

<br>

name: Generate Contribution Snake

on:
  schedule:
    # Ular akan ter-update otomatis setiap 12 jam
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v3
      - name: Generate Snake Animation
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
      - name: Push Snake to Output Branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          <!-- Snake Telemetry System -->
<div align="center">
  <br>
  <code style="color: #00F0FF;">> INITIATING_CONTRIBUTION_TRACKER...</code>
  <br>
  <img src="https://raw.githubusercontent.com/AgraZahranAgdyputra/AgraZahranAgdyputra/output/github-snake-dark.svg" alt="Contribution Snake" width="100%">
</div>
