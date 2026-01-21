<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Court 9 Badminton Center Queue Management System</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
        }
        
        body {
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
            padding: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .container {
            background-color: #161b22;
            border-radius: 8px;
            padding: 30px;
            border: 1px solid #30363d;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 1px solid #30363d;
        }
        
        h1 {
            color: #58a6ff;
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .subtitle {
            color: #8b949e;
            font-size: 1.2rem;
            margin-bottom: 20px;
        }
        
        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
            justify-content: center;
        }
        
        .badge {
            display: inline-block;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
        }
        
        .badge-laravel {
            background-color: #ff2d20;
            color: white;
        }
        
        .badge-tailwind {
            background-color: #06b6d4;
            color: white;
        }
        
        .badge-js {
            background-color: #f7df1e;
            color: #323330;
        }
        
        .badge-php {
            background-color: #777bb4;
            color: white;
        }
        
        section {
            margin-bottom: 30px;
        }
        
        h2 {
            color: #58a6ff;
            font-size: 1.8rem;
            margin-bottom: 15px;
            padding-bottom: 8px;
            border-bottom: 1px solid #30363d;
        }
        
        h3 {
            color: #79c0ff;
            font-size: 1.3rem;
            margin: 15px 0 10px;
        }
        
        p {
            margin-bottom: 15px;
        }
        
        ul, ol {
            padding-left: 20px;
            margin-bottom: 15px;
        }
        
        li {
            margin-bottom: 8px;
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }
        
        .feature-card {
            background-color: #21262d;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            transition: transform 0.2s, border-color 0.2s;
        }
        
        .feature-card:hover {
            transform: translateY(-3px);
            border-color: #58a6ff;
        }
        
        .feature-card h3 {
            margin-top: 0;
            display: flex;
            align-items: center;
        }
        
        .feature-icon {
            margin-right: 10px;
            font-size: 1.5rem;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 15px;
        }
        
        .tech-item {
            background-color: #21262d;
            padding: 10px 15px;
            border-radius: 6px;
            border: 1px solid #30363d;
            flex: 1;
            min-width: 150px;
            text-align: center;
        }
        
        .tech-item h4 {
            color: #79c0ff;
            margin-bottom: 5px;
        }
        
        .installation {
            background-color: #21262d;
            border-radius: 6px;
            padding: 20px;
            border-left: 4px solid #238636;
            margin-top: 15px;
        }
        
        code {
            background-color: #0d1117;
            color: #c9d1d9;
            padding: 2px 6px;
            border-radius: 4px;
            font-family: 'Courier New', monospace;
            font-size: 0.9rem;
            border: 1px solid #30363d;
        }
        
        pre {
            background-color: #0d1117;
            padding: 15px;
            border-radius: 6px;
            overflow-x: auto;
            margin: 15px 0;
            border: 1px solid #30363d;
        }
        
        pre code {
            background-color: transparent;
            border: none;
            padding: 0;
        }
        
        .screenshot {
            background-color: #21262d;
            border-radius: 6px;
            padding: 20px;
            text-align: center;
            border: 1px solid #30363d;
            margin: 20px 0;
        }
        
        .screenshot-placeholder {
            background-color: #0d1117;
            height: 300px;
            border-radius: 4px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #8b949e;
            border: 1px dashed #30363d;
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #30363d;
            color: #8b949e;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            body {
                padding: 10px;
            }
            
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .feature-grid {
                grid-template-columns: 1fr;
            }
            
            .tech-item {
                min-width: 100%;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>Court 9 Badminton Center Queue Management System</h1>
            <p class="subtitle">A comprehensive management system for badminton centers with matchmaking, e-commerce, stringing services, reservations, and tournament management.</p>
            
            <div class="badges">
                <span class="badge badge-laravel">Laravel</span>
                <span class="badge badge-tailwind">Tailwind CSS</span>
                <span class="badge badge-js">JavaScript</span>
                <span class="badge badge-php">PHP</span>
            </div>
        </header>
        
        <section id="overview">
            <h2><i class="fas fa-info-circle"></i> Overview</h2>
            <p>The Court 9 Badminton Center Queue Management System is a comprehensive web application designed to streamline operations for badminton centers. It integrates multiple functionalities into a single platform to manage player matchmaking, court reservations, e-commerce operations, stringing services, and tournament management.</p>
            
            <p>This system helps badminton centers optimize court usage, improve customer experience, and manage all business operations efficiently from a single dashboard.</p>
        </section>
        
        <section id="features">
            <h2><i class="fas fa-star"></i> Features</h2>
            <div class="feature-grid">
                <div class="feature-card">
                    <h3><span class="feature-icon">🏸</span> Matchmaking Rating</h3>
                    <p>Intelligent player matchmaking based on skill ratings, availability, and preferences. Implements an ELO-like rating system to ensure balanced and competitive matches.</p>
                </div>
                
                <div class="feature-card">
                    <h3><span class="feature-icon">🛒</span> E-Commerce (Point of Sales)</h3>
                    <p>Complete POS system for managing sales of badminton equipment, merchandise, and court bookings. Includes inventory management, sales reports, and payment processing integration.</p>
                </div>
                
                <div class="feature-card">
                    <h3><span class="feature-icon">🎾</span> Stringing Services</h3>
                    <p>Manage racquet stringing requests with service tracking, pricing, and scheduling. Customers can select string types, tension preferences, and track completion status.</p>
                </div>
                
                <div class="feature-card">
                    <h3><span class="feature-icon">📅</span> Reservation System</h3>
                    <p>Interactive court reservation system with real-time availability, automated scheduling, and payment integration. Supports recurring bookings and group reservations.</p>
                </div>
                
                <div class="feature-card">
                    <h3><span class="feature-icon">🏆</span> Club Tournaments System</h3>
                    <p>Organize and manage tournaments with automated bracket generation, participant registration, score tracking, and result publishing. Supports different tournament formats.</p>
                </div>
                
                <div class="feature-card">
                    <h3><span class="feature-icon">📊</span> Admin Dashboard</h3>
                    <p>Comprehensive dashboard for administrators to monitor all operations, generate reports, manage users, and configure system settings.</p>
                </div>
            </div>
        </section>
        
        <section id="tech-stack">
            <h2><i class="fas fa-code"></i> Technology Stack</h2>
            <div class="tech-stack">
                <div class="tech-item">
                    <h4>Backend</h4>
                    <p>Laravel 9+</p>
                    <p>PHP 8.1+</p>
                    <p>MySQL</p>
                </div>
                
                <div class="tech-item">
                    <h4>Frontend</h4>
                    <p>Tailwind CSS</p>
                    <p>JavaScript (ES6+)</p>
                    <p>Alpine.js / Vue.js</p>
                </div>
                
                <div class="tech-item">
                    <h4>Other Tools</h4>
                    <p>Composer</p>
                    <p>npm / Yarn</p>
                    <p>Git</p>
                </div>
            </div>
        </section>
        
        <section id="installation">
            <h2><i class="fas fa-download"></i> Installation</h2>
            <div class="installation">
                <h3>Prerequisites</h3>
                <ul>
                    <li>PHP >= 8.1</li>
                    <li>Composer</li>
                    <li>Node.js & npm</li>
                    <li>MySQL >= 5.7</li>
                </ul>
                
                <h3>Setup Instructions</h3>
                <ol>
                    <li>Clone the repository:
                        <pre><code>git clone https://github.com/yourusername/court9-badminton-system.git
cd court9-badminton-system</code></pre>
                    </li>
                    <li>Install PHP dependencies:
                        <pre><code>composer install</code></pre>
                    </li>
                    <li>Install JavaScript dependencies:
                        <pre><code>npm install</code></pre>
                    </li>
                    <li>Copy environment file and configure:
                        <pre><code>cp .env.example .env</code></pre>
                    </li>
                    <li>Generate application key:
                        <pre><code>php artisan key:generate</code></pre>
                    </li>
                    <li>Configure your database in <code>.env</code> file</li>
                    <li>Run migrations and seeders:
                        <pre><code>php artisan migrate --seed</code></pre>
                    </li>
                    <li>Build frontend assets:
                        <pre><code>npm run build</code></pre>
                    </li>
                    <li>Start the development server:
                        <pre><code>php artisan serve</code></pre>
                    </li>
                </ol>
            </div>
        </section>
        
        <section id="screenshots">
            <h2><i class="fas fa-images"></i> Screenshots</h2>
            <div class="screenshot">
                <div class="screenshot-placeholder">
                    <div>
                        <i class="fas fa-camera fa-3x"></i>
                        <p>Screenshots will be added soon</p>
                    </div>
                </div>
                <p><em>Dashboard preview - Coming soon</em></p>
            </div>
        </section>
        
        <section id="contributing">
            <h2><i class="fas fa-hands-helping"></i> Contributing</h2>
            <p>Contributions are welcome! Please feel free to submit a Pull Request.</p>
            <ol>
                <li>Fork the repository</li>
                <li>Create your feature branch (<code>git checkout -b feature/AmazingFeature</code>)</li>
                <li>Commit your changes (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
                <li>Push to the branch (<code>git push origin feature/AmazingFeature</code>)</li>
                <li>Open a Pull Request</li>
            </ol>
        </section>
        
        <footer>
            <p>Court 9 Badminton Center Queue Management System &copy; 2023</p>
            <p>Built with Laravel, Tailwind CSS, and JavaScript</p>
        </footer>
    </div>

    <script>
        // Simple script to make feature cards interactive
        document.addEventListener('DOMContentLoaded', function() {
            const featureCards = document.querySelectorAll('.feature-card');
            
            featureCards.forEach(card => {
                card.addEventListener('click', function() {
                    this.style.transform = 'translateY(-5px)';
                    setTimeout(() => {
                        this.style.transform = 'translateY(-3px)';
                    }, 150);
                });
            });
            
            // Add copy functionality to code blocks
            const codeBlocks = document.querySelectorAll('pre');
            codeBlocks.forEach(block => {
                block.addEventListener('click', function() {
                    const code = this.querySelector('code').innerText;
                    navigator.clipboard.writeText(code).then(() => {
                        const originalBorder = this.style.border;
                        this.style.border = '2px solid #238636';
                        this.style.backgroundColor = '#0d4217';
                        
                        setTimeout(() => {
                            this.style.border = originalBorder;
                            this.style.backgroundColor = '';
                        }, 1000);
                    });
                });
            });
        });
    </script>
</body>
</html>
