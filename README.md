# ThinTrack-Forest

ThinTrack-Forest is an open-source project that aims to develop a method to translate forest management rules into Relative Density Index curve usable in land surface models such as ORCHIDEE. The project is implemented in Julia programming language and is designed to process forest yield tables and forester reference manuals to extract meaningful information about forest thinning and types. The project includes functionality to generate thinning trajectories and evaluate the performance of the application.

## Features

- Translation of forest management rules into Relative Density Index curve usable in land surface models such as ORCHIDEE.
- Integration of polynomial curve fitting for generating thinning trajectories.
- Experiment setup for evaluating the performance of the application.
- Web app deployment on Heroku.

## File structure

The `ThinTrack-Forest` repository is organized into several files and directories:

- `app.jl`: main application file for generating and plotting thinning trajectories.
- `thinning_trajectories.jl`: module for generating thinning trajectories based on forest yield tables and forester reference manuals using polynomial curve fitting.
- `forest_def.jl`: module for defining the forest types used in the application.
- `Parameters.jl`: module for defining global parameters used throughout the application.
- `Experiment_setup.jl`: module for setting up and running experiments to evaluate the performance of the application.
- `data`: directory for storing forest yield tables and forester reference manuals used in the application.
- `experiments`: directory for storing results of experiments.
- `utils`: directory for utility functions used throughout the application.
- `Procfile`: file for declaring the commands that are executed by the app on startup.
- `Project.toml` and `Manifest.toml`: files for managing the project's dependencies.
- `run.jl`: file for running the application locally.

## Usage

To use the ThinTrack-Forest application, follow these steps:

1. Clone the repository to your local machine.
2. Install the required Julia packages listed in the `Project.toml` file using the `Pkg` package manager.
3. Prepare your forest yield tables and forester reference manuals and store them in the `data` directory.
4. Adjust the global parameters defined in `Parameters.jl` to match your data and analysis needs.
5. Run the application using the `app.jl` file to generate and plot thinning trajectories.

You can also use the `Experiment_setup.jl` file to set up and run experiments to evaluate the performance of the application. The results of these experiments will be stored in the `experiments` directory.

The web app deployment of ThinTrack-Forest is available on Heroku at https://thintrack-forest.herokuapp.com/.

## License

ThinTrack-Forest is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

If you have any questions or suggestions regarding ThinTrack-Forest, please contact the project owner: [volarex84](https://github.com/volarex84).
