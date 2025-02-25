# in-class-game
:root {
    --hud-bg-color: rgba(0, 0, 0, 0.7);
    --inventory-slot-size: 60px;
}

body {
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: var(--bs-dark);
}

.game-container {
    position: relative;
    width: 100vw;
    height: 100vh;
}

#gameCanvas {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.hud {
    position: absolute;
    top: 20px;
    left: 20px;
    z-index: 1000;
}

.health-bar {
    width: 200px;
    margin-bottom: 10px;
}

.score {
    color: var(--bs-light);
    font-size: 1.2em;
    margin-bottom: 10px;
}

.mini-map {
    width: 150px;
    height: 150px;
    background: var(--hud-bg-color);
    border: 2px solid var(--bs-secondary);
    border-radius: 5px;
}

.inventory {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    z-index: 1000;
}

.inventory-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
    padding: 10px;
    background: var(--hud-bg-color);
    border-radius: 5px;
}

.inventory-slot {
    width: var(--inventory-slot-size);
    height: var(--inventory-slot-size);
    background: rgba(255, 255, 255, 0.1);
    border: 2px solid var(--bs-secondary);
    border-radius: 5px;
}

.controls-overlay {
    position: absolute;
    top: 20px;
    right: 20px;
    padding: 15px;
    background: var(--hud-bg-color);
    border-radius: 5px;
    color: var(--bs-light);
    z-index: 1000;
}

.controls-info p {
    margin: 5px 0;
    font-size: 0.9em;
}
