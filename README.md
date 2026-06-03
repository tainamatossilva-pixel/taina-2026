# taina-2026
/* Configurações Gerais / Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    scroll-behavior: smooth;
}

:root {
    --verde: #2E6F40;
    --marrom: #4A3B32;
    --azul: #1D4ED8;
    --claro: #F8FAFC;
    --escuro: #1E293B;
    --branco: #FFFFFF;
}

body {
    background-color: var(--branco);
    color: var(--escuro);
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Botões */
.btn {
    display: inline-block;
    padding: 12px 28px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    cursor: pointer;
    border: none;
}

.btn-green { background-color: var(--verde); color: var(--branco); }
.btn-green:hover { background-color: #22522e; transform: translateY(-2px); }

.btn-blue { background-color: var(--azul); color: var(--branco); }
.btn-blue:hover { background-color: #113aafd; transform: translateY(-2px); }

.btn-outline { border: 2px solid var(--branco); color: var(--branco); background: transparent; }
.btn-outline:hover { background-color: var(--branco); color: var(--escuro); }

/* Menu Superior */
header {
    background-color: rgba(255, 255, 255, 0.95);
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;
}

.logo {
    font-size: 24px;
    font-weight: 700;
    color: var(--marrom);
}

.logo i { color: var(--verde); }
.logo span { color: var(--verde); }

.nav-links {
    display: flex;
    list-style: none;
    gap: 30px;
}

.nav-links a {
    text-decoration: none;
    color: var(--escuro);
    font-weight: 500;
    transition: color 0.3s;
}

.nav-links a:hover, .nav-links a.active {
    color: var(--verde);
}

.menu-toggle {
    display: none;
    font-size: 24px;
    cursor: pointer;
}

/* Banner Principal (Hero) */
.hero-section {
    background: linear-gradient(rgba(46, 111, 64, 0.7), rgba(74, 59, 50, 0.8)), 
                url('https://images.unsplash.com/photo-1530595467537-0b5996c41f2d?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
    height: 100vh;
    display: flex;
    align-items: center;
    color: var(--branco);
    padding-top: 80px;
    text-align: center;
}

.hero-content {
    max-width: 800px;
}

.hero-content h1 {
    font-size: 48px;
    margin-bottom: 20px;
    font-weight: 800;
}

.hero-content p {
    font-size: 20px;
    margin-bottom: 40px;
    opacity: 0.9;
}

.hero-buttons {
    display: flex;
    gap: 20px;
    justify-content: center;
}

/* Seção Sobre */
.about-section {
    padding: 100px 20px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 50px;
    align-items: center;
}

.about-text h2 {
    font-size: 36px;
    color: var(--marrom);
    margin-bottom: 20px;
}

.about-text p {
    margin-bottom: 30px;
    color: #475569;
}

.stats {
    display: flex;
    gap: 30px;
}

.stat-item h3 {
    color: var(--verde);
    font-size: 24px;
}

.about-image {
    width: 100%;
    height: 350px;
}

.image-placeholder {
    background: linear-gradient(135deg, var(--verde), var(--azul));
    width: 100%;
    height: 100%;
    border-radius: 20px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: var(--branco);
}

.image-placeholder i {
    font-size: 60px;
    margin-bottom: 15px;
}

/* Cards dos Pilares */
.pillars-section {
    background-color: var(--claro);
    padding: 100px 20px;
}

.section-title {
    text-align: center;
    font-size: 36px;
    margin-bottom: 60px;
    color: var(--marrom);
}

.cards-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.card {
    background-color: var(--branco);
    padding: 40px 30px;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.02);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.06);
}

.card-icon {
    width: 60px;
    height: 60px;
    border-radius: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 24px;
    margin-bottom: 25px;
}

.icon-green { background-color: rgba(46, 111, 64, 0.1); color: var(--verde); }
.icon-blue { background-color: rgba(29, 78, 216, 0.1); color: var(--azul); }
.icon-brown { background-color: rgba(74, 59, 50, 0.1); color: var(--marrom); }

.card h3 {
    margin-bottom: 15px;
    color: var(--escuro);
}

/* Formulário de Contato */
.contact-section {
    padding: 100px 20px;
    text-align: center;
    max-width: 600px !important;
}

.contact-section h2 { font-size: 36px; color: var(--marrom); margin-bottom: 15px;}
.contact-section p { color: #64748B; margin-bottom: 40px; }

.contact-form .form-group {
    margin-bottom: 20px;
}

.contact-form input, .contact-form textarea {
    width: 100%;
    padding: 15px 20px;
    border: 2px solid #E2E8F0;
    border-radius: 8px;
    outline: none;
    font-size: 16px;
    transition: border-color 0.3s;
}

.contact-form input:focus, .contact-form textarea:focus {
    border-color: var(--verde);
}

/* Rodapé */
footer {
    background-color: var(--marrom);
    color: var(--branco);
    padding: 60px 20px 20px;
    text-align: center;
}

.footer-container p {
    opacity: 0.8;
    margin: 10px 0 20px;
}

.footer-logo {
    font-size: 26px;
    font-weight: 700;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-bottom: 40px;
}

.social-links a {
    color: var(--branco);
    font-size: 20px;
    opacity: 0.8;
    transition: opacity 0.3s;
}

.social-links a:hover { opacity: 1; color