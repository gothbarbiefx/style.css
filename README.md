# style.css
style
@font-face {
  font-family: "Pixel";
  src: url("pixel-font.woff2");
}

body {
  margin: 0;
  color: #7cff00;
  background:
    repeating-linear-gradient(
      0deg,
      rgba(255, 0, 170, 0.08) 0 1px,
      transparent 1px 4px
    ),
    #09000f;
  font-family: "Pixel", monospace;
}

h1 {
  position: relative;
  font-size: clamp(3rem, 14vw, 9rem);
  text-shadow: 5px 0 #ff00aa, -5px 0 #00eaff;
  animation: glitch 700ms steps(2) infinite;
}

.ticket-button {
  position: sticky;
  bottom: 1rem;
  display: block;
  margin: 2rem auto;
  padding: 1.2rem;
  color: #09000f;
  background: #7cff00;
  border: 4px solid white;
  box-shadow: 8px 8px 0 #ff00aa;
  text-align: center;
}

@keyframes glitch {
  0%, 88%, 100% { transform: translate(0); }
  90% { transform: translate(4px, -2px); }
  94% { transform: translate(-3px, 3px); }
}
