---
layout: page
title: Simulations
permalink: /simulations/
---

## Statics Simulations

Interactive sandboxes I built for PHYS-291 Statics. Each one runs in your browser (no install, no login, nothing is recorded). Click a card to open the simulation.

<style>
.sim-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
  gap: 20px;
  margin: 20px 0;
}
.sim-card {
  display: flex;
  flex-direction: column;
  border: 1px solid #ddd;
  border-radius: 6px;
  overflow: hidden;
  background: #fff;
  color: inherit;
  text-decoration: none;
  transition: box-shadow 0.15s, transform 0.15s, border-color 0.15s;
}
.sim-card:hover,
.sim-card:focus {
  border-color: #2a7ae2;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.18);
  transform: translateY(-2px);
  text-decoration: none;
}
.sim-card:active {
  transform: translateY(0);
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.2);
}
.sim-card img {
  display: block;
  width: 100%;
  aspect-ratio: 3 / 2;
  object-fit: cover;
  object-position: top left;
  border-bottom: 1px solid #ddd;
  background: #f7f7f7;
}
.sim-card .sim-body { padding: 10px 14px 14px; }
.sim-card h3 { margin: 0 0 6px; font-size: 18px; color: #2a7ae2; }
.sim-card p { margin: 0; font-size: 14px; line-height: 1.4; color: #424242; }
.sim-source { font-size: 13px; color: #828282; }
/* A cell holding a card plus a quiet second link beneath it (a link cannot nest inside the card). */
.sim-cell { display: flex; flex-direction: column; }
.sim-cell .sim-card { flex: 1 1 auto; }
.sim-alt { margin: 6px 2px 0; font-size: 13px; line-height: 1.35; color: #666; }
</style>

<div class="sim-grid">

  <a class="sim-card" href="https://zimmermant.github.io/point-particle-statics/">
    <img src="/img/simulations/point-particle-statics.png" alt="Screenshot: a ring held by two ropes and a hanging crate, with its free-body diagram and force triangle" loading="lazy">
    <div class="sim-body">
      <h3>Three Ropes, One Ring</h3>
      <p>Drag the rope angles or the force arrows and watch the tensions resolve live in a three-force equilibrium at a point.</p>
    </div>
  </a>

  <a class="sim-card" href="https://zimmermant.github.io/ball-on-ramp-statics/">
    <img src="/img/simulations/ball-on-ramp-statics.png" alt="Screenshot: a ball on a ramp held by a flap, with its free-body diagram" loading="lazy">
    <div class="sim-body">
      <h3>A Ball on a Ramp</h3>
      <p>Change the ramp angle and the flap angle, and see how the two contact forces are fixed by the geometry.</p>
    </div>
  </a>

  <a class="sim-card" href="https://zimmermant.github.io/crate-over-pulley-statics/">
    <img src="/img/simulations/crate-over-pulley-statics.png" alt="Screenshot: a crate hanging from a rope over a pulley, with a support rope to the ceiling" loading="lazy">
    <div class="sim-body">
      <h3>A Crate over a Pulley</h3>
      <p>Slide the ground anchor and see that the support rope's angle doesn't depend on the crate's weight.</p>
    </div>
  </a>

  <a class="sim-card" href="https://zimmermant.github.io/torque-i-beam/">
    <img src="/img/simulations/torque-i-beam.png" alt="Screenshot: an I-beam with a force arrow and a pivot marked on it" loading="lazy">
    <div class="sim-body">
      <h3>Torque on an I-Beam</h3>
      <p>Place a force, choose a pivot, draw the lever arm, and predict which way the beam will turn.</p>
    </div>
  </a>

  <a class="sim-card" href="https://zimmermant.github.io/distributed-load-beam/">
    <img src="/img/simulations/distributed-load-beam.png" alt="Screenshot: a wall-mounted beam with rectangular and triangular distributed loads and their equivalent forces" loading="lazy">
    <div class="sim-body">
      <h3>Distributed Load on a Beam</h3>
      <p>Adjust a rectangular and a triangular load and watch the equivalent forces and their locations change.</p>
    </div>
  </a>

  <div class="sim-cell">
    <a class="sim-card" href="https://zimmermant.github.io/beam-and-two-force-link/">
      <img src="/img/simulations/beam-and-two-force-link.png" alt="Screenshot: a beam held by a pin at one end and a slanted two-force link at the other, with its free-body diagram, the beam drawn as a single point, and the three forces as a closed polygon" loading="lazy">
      <div class="sim-body">
        <h3>A Beam on a Pin and a Link</h3>
        <p>Drag the load and watch the free-body diagram, the three lines of action meeting at a point, and the force polygon all follow.</p>
      </div>
    </a>
    <p class="sim-alt"><a href="https://zimmermant.github.io/beam-and-two-force-link/dist/beam_link_fbd_display.html">Diagrams only</a> — the same four diagrams with no controls, for projecting.</p>
  </div>

  <a class="sim-card" href="https://zimmermant.github.io/beam-on-roller-and-collar/">
    <img src="/img/simulations/beam-on-roller-and-collar.png" alt="Screenshot: a beam on a roller at one end and a collar on a vertical shaft at the other, with an applied couple, shown as a free-body diagram, as a single point, and as a force polygon" loading="lazy">
    <div class="sim-body">
      <h3>A Beam on a Roller and a Collar</h3>
      <p>Drag the load and turn the applied couple. The collar resists turning, so one of the three unknowns is a couple — and the force polygon closes without it.</p>
    </div>
  </a>

</div>

<p class="sim-source">Source code for each simulation is on my <a href="https://github.com/zimmermant?tab=repositories">GitHub</a> page, under an MIT license.</p>
