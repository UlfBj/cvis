# Axle features
The axle features defined in the AxleFeature directory are typically related to trucks and not directly to passenger cars.
In order to not 'bloat' the passenger car centric VSS vspec tree a separate truck vspec tree is created.
It is identical to the VSS tree except for the Chassis vspec file that is extended with include directives for the axle features in the AxleFeature directory (which is not found in the VSS vspec directory structure).

If the Axlefeature is configured to NONE the Truck vspec tree can be used to generate an output tree that is identical to the standard passenger car (VSS) tree with the only difference being the root node name Truck instead of Vehicle. This can obviously be fixed by updating the root node name in the root vspec file.

The Profile/Truck/Chassis/Chassis.vspec overlay file shall be added to the vspec CLI command as shown below:

vspec export yaml -u Vehicle/Car/units.yaml -q Vehicle/Car/quantities.yaml -l Profile/Truck/Chassis/Chassis.vspec -l Config/Truck/truck.vspec -s Vehicle/Car/VehicleSignalSpecification.vspec -o truck.yaml

The vspecPreprocessor does currently not display this overlay addition in the exporter command that it displays.
