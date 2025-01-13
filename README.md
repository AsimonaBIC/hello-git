# hello-git

.section-projects {
    position: relative;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 4rem 2rem;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 3rem;
    max-width: 1400px;
    width: 100%;
}

.project-card {
    position: relative;
    background: rgba(255, 255, 255, 0.03);
    backdrop-filter: blur(10px);
    border-radius: 20px;
    border: 1px solid rgba(255, 255, 255, 0.1);
    padding: 2rem;
    transition: all 0.4s ease;
    opacity: 0;
    animation: fadeUpProject 0.8s ease-out forwards;
}

.project-card:nth-child(2) {
    animation-delay: 0.2s;
}

.project-card:nth-child(3) {
    animation-delay: 0.4s;
}

.project-card:hover {
    transform: translateY(-10px);
    border-color: rgba(255, 255, 255, 0.2);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}

.project-image {
    width: 100%;
    height: 200px;
    border-radius: 12px;
    overflow: hidden;
    margin-bottom: 1.5rem;
}

.project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.6s ease;
}

.project-card:hover .project-image img {
    transform: scale(1.1);
}

.project-content h3 {
    color: #fff;
    font-size: 1.5rem;
    margin-bottom: 1rem;
    font-family: 'Space Grotesk', sans-serif;
}

.project-content p {
    color: rgba(255, 255, 255, 0.7);
    font-size: 1rem;
    line-height: 1.6;
}

.section-title {
    font-family: 'Space Grotesk', sans-serif;
    font-size: clamp(3rem, 5vw, 5rem);
    text-align: center;
    margin-bottom: 4rem;
    width: 100%;
    background: linear-gradient(to right, #fff, #919191);
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
}

<section class="section section-projects">
            <h2 class="section-title">My Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-image">
                    </div>
                    <div class="project-content">
                        <h3>Project Title</h3>
                        <p>Project description goes here. Explain what technologies you used and what you learned.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                    </div>
                    <div class="project-content">
                        <h3>Project Title</h3>
                        <p>Project description goes here. Explain what technologies you used and what you learned.</p>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-image">
                    </div>
                    <div class="project-content">
                        <h3>Project Title</h3>
                        <p>Project description goes here. Explain what technologies you used and what you learned.</p>
                    </div>
                </div>
                <!-- Repeat for other cards -->
            </div>
        </section>
