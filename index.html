(function() {
  // ---- Particle Background ----
  const canvas = document.getElementById('particleCanvas');
  const ctx = canvas.getContext('2d');
  let particlesArray = [];
  const numberOfParticles = 100;

  function resizeCanvas() {
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;
  }
  resizeCanvas();
  window.addEventListener('resize', resizeCanvas);

  class Particle {
    constructor() {
      this.x = Math.random() * canvas.width;
      this.y = Math.random() * canvas.height;
      this.size = Math.random() * 2 + 0.5;
      this.speedX = Math.random() * 0.5 - 0.25;
      this.speedY = Math.random() * 0.5 - 0.25;
    }
    update() {
      this.x += this.speedX;
      this.y += this.speedY;
      if (this.x < 0 || this.x > canvas.width) this.speedX *= -1;
      if (this.y < 0 || this.y > canvas.height) this.speedY *= -1;
    }
    draw() {
      ctx.fillStyle = 'rgba(109,93,252,0.15)';
      ctx.beginPath();
      ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
      ctx.fill();
    }
  }

  function createParticles() {
    particlesArray = [];
    for (let i = 0; i < numberOfParticles; i++) {
      particlesArray.push(new Particle());
    }
  }
  createParticles();

  function connectParticles() {
    for (let a = 0; a < particlesArray.length; a++) {
      for (let b = a + 1; b < particlesArray.length; b++) {
        let dx = particlesArray[a].x - particlesArray[b].x;
        let dy = particlesArray[a].y - particlesArray[b].y;
        let distance = Math.sqrt(dx*dx + dy*dy);
        if (distance < 120) {
          ctx.strokeStyle = `rgba(109,93,252,${0.08 - distance/1500})`;
          ctx.lineWidth = 0.5;
          ctx.beginPath();
          ctx.moveTo(particlesArray[a].x, particlesArray[a].y);
          ctx.lineTo(particlesArray[b].x, particlesArray[b].y);
          ctx.stroke();
        }
      }
    }
  }

  function animateParticles() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    particlesArray.forEach(p => { p.update(); p.draw(); });
    connectParticles();
    requestAnimationFrame(animateParticles);
  }
  animateParticles();

  // ---- Scroll Reveal ----
  const revealElements = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('active');
        // animate skill bars
        entry.target.querySelectorAll('.fill').forEach(fill => {
          if (fill.dataset.width) fill.style.width = fill.dataset.width + '%';
        });
      }
    });
  }, { threshold: 0.15 });
  revealElements.forEach(el => observer.observe(el));

  // ---- Typewriter (only on home page if .typewriter exists) ----
  const typedEl = document.querySelector('.typewriter');
  if (typedEl) {
    const fullText = typedEl.textContent;
    typedEl.textContent = '';
    let idx = 0;
    function type() {
      if (idx < fullText.length) {
        typedEl.textContent += fullText.charAt(idx);
        idx++;
        setTimeout(type, 50);
      }
    }
    type();
  }

  // ---- Active nav link based on current page ----
  const currentPath = window.location.pathname.split('/').pop() || 'index.html';
  document.querySelectorAll('.nav-links a').forEach(link => {
    if (link.getAttribute('href') === currentPath) {
      link.classList.add('active');
    }
  });
})();
