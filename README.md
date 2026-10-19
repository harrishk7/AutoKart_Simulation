# AutoKart Simulation

Simulation source for the AutoKart browser lab and Python/ROS 2/Gazebo simulator.
This repository does not authorize vehicle motion.

## Browser Algorithm Lab

```bash
cd phase_sim
npm ci
npm run dev:lab
```

Open <http://localhost:5181/mission>, choose a scenario, and press **RUN**.
The default sandbox runs locally in the browser. The Python Core Lab and ROS
simulation source require their separate services; see
[phase_sim/README.md](phase_sim/README.md) for the data modes and limitations.

Run the frontend checks with `npm run check` from `phase_sim/`.

## Python simulator

```bash
cd kart
./scripts/setup.sh
./scripts/test.sh
```

See [kart/README.md](kart/README.md) for the CLI, dashboard, ROS 2 and Gazebo
entry points. ROS 2 and Gazebo require their own installed dependencies.

Generated builds, installed dependencies, telemetry runs, and large artifacts
are intentionally excluded from this source repository.
