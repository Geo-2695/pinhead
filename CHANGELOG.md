# Changelog

## [16.26.0] - 2026-10-19

_Pinhead v26_

⚠️ This is a major Pinhead release that may cause breaking changes for a subset of downstream users.

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the `changelog.json` file included in the distribution. For a simple mapping of old IDs to new IDs, see `id_upgrades.json`.

### Structural changes affecting the distributed files

* Icon IDs may now start with a number character 0-9 (e.g. `1_plus.svg`).
* Repos listed in `external_sources.json` may now specify specific branches or commits.
* A new file `id_upgrades.json` has been added. It provides simple upgrade paths for icon IDs in the format `"historical_id": "latest_id"`.
* A new file `id_metadata.json` has been added. It provides data for sorting the icons into categories based on their IDs.

### Structural changes affecting the repository

* The `metadata/changelog.json` file has been broken up into one file per release. See the `metadata/changelogs` directory.
* The `icons` repo directory has been flattened and no longer contains subfolders.

### Renamed and redesigned icons (58)

* <img src="https://pinhead.ink/v25/city_gate.svg" width="15px"> **city\_gate** -> <img src="https://pinhead.ink/v26/wall_with_battlement_and_sallyport.svg" width="15px"> **wall\_with\_battlement\_and\_sallyport** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/phone_top_right_with_plus.svg" width="15px"> **phone\_top\_right\_with\_plus** -> <img src="https://pinhead.ink/v26/phone_top_right_and_plus.svg" width="15px"> **phone\_top\_right\_and\_plus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/gable_roofed_shelter_with_spoon_and_knife.svg" width="15px"> **gable\_roofed\_shelter\_with\_spoon\_and\_knife** -> <img src="https://pinhead.ink/v26/spoon_beside_table_knife_in_gable_roofed_shelter.svg" width="15px"> **spoon\_beside\_table\_knife\_in\_gable\_roofed\_shelter** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cup_and_saucer.svg" width="15px"> **cup\_and\_saucer** -> <img src="https://pinhead.ink/v26/handled_teacup_and_saucer.svg" width="15px"> **handled\_teacup\_and\_saucer** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cup_and_saucer_and_wifi.svg" width="15px"> **cup\_and\_saucer\_and\_wifi** -> <img src="https://pinhead.ink/v26/handled_teacup_and_saucer_and_wifi.svg" width="15px"> **handled\_teacup\_and\_saucer\_and\_wifi** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cup_and_saucer_and_pawprint.svg" width="15px"> **cup\_and\_saucer\_and\_pawprint** -> <img src="https://pinhead.ink/v26/handled_teacup_and_saucer_and_pawprint.svg" width="15px"> **handled\_teacup\_and\_saucer\_and\_pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/lowrise_building_and_tree_on_ground.svg" width="15px"> **lowrise\_building\_and\_tree\_on\_ground** -> <img src="https://pinhead.ink/v26/lowrise_building_beside_lollipop_tree_on_ground.svg" width="15px"> **lowrise\_building\_beside\_lollipop\_tree\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/plane_takeoff_above_ground.svg" width="15px"> **plane\_takeoff\_above\_ground** -> <img src="https://pinhead.ink/v26/plane_ascending_above_ground.svg" width="15px"> **plane\_ascending\_above\_ground** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v25/seaplane_takeoff_above_water.svg" width="15px"> **seaplane\_takeoff\_above\_water** -> <img src="https://pinhead.ink/v26/seaplane_ascending_above_water.svg" width="15px"> **seaplane\_ascending\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v25/person_with_droplets.svg" width="15px"> **person\_with\_droplets** -> <img src="https://pinhead.ink/v26/person_standing_with_droplets.svg" width="15px"> **person\_standing\_with\_droplets** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230), [#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/person_with_open_arms.svg" width="15px"> **person\_with\_open\_arms** -> <img src="https://pinhead.ink/v26/person_standing_open_armed.svg" width="15px"> **person\_standing\_open\_armed** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/person_reaching_up.svg" width="15px"> **person\_reaching\_up** -> <img src="https://pinhead.ink/v26/person_standing_reaching_up.svg" width="15px"> **person\_standing\_reaching\_up** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/womens_restroom_symbol.svg" width="15px"> **womens\_restroom\_symbol** -> <img src="https://pinhead.ink/v26/person_standing_wearing_dress.svg" width="15px"> **person\_standing\_wearing\_dress** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/mens_restroom_symbol.svg" width="15px"> **mens\_restroom\_symbol** -> <img src="https://pinhead.ink/v26/broadshouldered_person_standing.svg" width="15px"> **broadshouldered\_person\_standing** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/womens_and_mens_restroom_symbol.svg" width="15px"> **womens\_and\_mens\_restroom\_symbol** -> <img src="https://pinhead.ink/v26/person_standing_wearing_dress_beside_broadshouldered_person_standing.svg" width="15px"> **person\_standing\_wearing\_dress\_beside\_broadshouldered\_person\_standing** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/womens_and_mens_separate_restrooms_symbol.svg" width="15px"> **womens\_and\_mens\_separate\_restrooms\_symbol** -> <img src="https://pinhead.ink/v26/person_standing_wearing_dress_beside_divider_beside_broadshouldered_person_standing.svg" width="15px"> **person\_standing\_wearing\_dress\_beside\_divider\_beside\_broadshouldered\_person\_standing** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/family_restroom_symbol.svg" width="15px"> **family\_restroom\_symbol** -> <img src="https://pinhead.ink/v26/person_standing_wearing_dress_beside_child_standing_beside_broadshouldered_person_standing.svg" width="15px"> **person\_standing\_wearing\_dress\_beside\_child\_standing\_beside\_broadshouldered\_person\_standing** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/elevator_rider.svg" width="15px"> **elevator\_rider** -> <img src="https://pinhead.ink/v26/person_standing_in_rectangle_outline_under_arrow_up_beside_arrow_down.svg" width="15px"> **person\_standing\_in\_rectangle\_outline\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/elevator_three_riders.svg" width="15px"> **elevator\_three\_riders** -> <img src="https://pinhead.ink/v26/three_people_standing_in_rectangle_outline_under_arrow_up_beside_arrow_down.svg" width="15px"> **three\_people\_standing\_in\_rectangle\_outline\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/phone_top_right_with_greek_cross.svg" width="15px"> **phone\_top\_right\_with\_greek\_cross** -> <img src="https://pinhead.ink/v26/phone_top_right_and_greek_cross.svg" width="15px"> **phone\_top\_right\_and\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/sitting_tank_toilet_with_droplet.svg" width="15px"> **sitting\_tank\_toilet\_with\_droplet** -> <img src="https://pinhead.ink/v26/sitting_tank_toilet_and_droplet.svg" width="15px"> **sitting\_tank\_toilet\_and\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/phone_right_with_exclamation_point.svg" width="15px"> **phone\_right\_with\_exclamation\_point** -> <img src="https://pinhead.ink/v26/phone_right_beside_exclamation_point.svg" width="15px"> **phone\_right\_beside\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/hand_holding_heart.svg" width="15px"> **hand\_holding\_heart** -> <img src="https://pinhead.ink/v26/heart_above_outstretched_hand.svg" width="15px"> **heart\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/tree_and_bench_with_backrest.svg" width="15px"> **tree\_and\_bench\_with\_backrest** -> <img src="https://pinhead.ink/v26/tree_beside_bench_with_backrest.svg" width="15px"> **tree\_beside\_bench\_with\_backrest** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cc_text.svg" width="15px"> **cc\_text** -> <img src="https://pinhead.ink/v26/cc_uppercase.svg" width="15px"> **cc\_uppercase** by [@quincylvania](https://github.com/quincylvania) ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v25/oc_text.svg" width="15px"> **oc\_text** -> <img src="https://pinhead.ink/v26/oc_uppercase.svg" width="15px"> **oc\_uppercase** by [@quincylvania](https://github.com/quincylvania) ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v25/wc_text.svg" width="15px"> **wc\_text** -> <img src="https://pinhead.ink/v26/wc_uppercase.svg" width="15px"> **wc\_uppercase** by [@quincylvania](https://github.com/quincylvania) ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v25/nine_one_one.svg" width="15px"> **nine\_one\_one** -> <img src="https://pinhead.ink/v26/911.svg" width="15px"> **911** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/conveyor_with_chevrons_right.svg" width="15px"> **conveyor\_with\_chevrons\_right** -> <img src="https://pinhead.ink/v26/three_chevrons_right_above_conveyor_belt.svg" width="15px"> **three\_chevrons\_right\_above\_conveyor\_belt** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/p_wide_with_arrow_right.svg" width="15px"> **p\_wide\_with\_arrow\_right** -> <img src="https://pinhead.ink/v26/wide_p_with_arrow_right.svg" width="15px"> **wide\_p\_with\_arrow\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/p_wide_with_arrow_bottom_right.svg" width="15px"> **p\_wide\_with\_arrow\_bottom\_right** -> <img src="https://pinhead.ink/v26/wide_p_with_arrow_bottom_right.svg" width="15px"> **wide\_p\_with\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/e_wide_with_arrow_right.svg" width="15px"> **e\_wide\_with\_arrow\_right** -> <img src="https://pinhead.ink/v26/wide_e_with_arrow_right.svg" width="15px"> **wide\_e\_with\_arrow\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/e_wide_with_arrow_bottom_right.svg" width="15px"> **e\_wide\_with\_arrow\_bottom\_right** -> <img src="https://pinhead.ink/v26/wide_e_with_arrow_bottom_right.svg" width="15px"> **wide\_e\_with\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/chicane_arrow.svg" width="15px"> **chicane\_arrow** -> <img src="https://pinhead.ink/v26/chicane_arrow_up.svg" width="15px"> **chicane\_arrow\_up** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/triangle_up.svg" width="15px"> **triangle\_up** -> <img src="https://pinhead.ink/v26/rounded_triangle_up.svg" width="15px"> **rounded\_triangle\_up** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/triangle_up_with_exclamation_point.svg" width="15px"> **triangle\_up\_with\_exclamation\_point** -> <img src="https://pinhead.ink/v26/rounded_triangle_up_with_exclamation_point.svg" width="15px"> **rounded\_triangle\_up\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/triangle_up_with_skull.svg" width="15px"> **triangle\_up\_with\_skull** -> <img src="https://pinhead.ink/v26/rounded_triangle_up_with_skull.svg" width="15px"> **rounded\_triangle\_up\_with\_skull** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/triangle_up_outline.svg" width="15px"> **triangle\_up\_outline** -> <img src="https://pinhead.ink/v26/rounded_triangle_up_outline.svg" width="15px"> **rounded\_triangle\_up\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/triangle_down.svg" width="15px"> **triangle\_down** -> <img src="https://pinhead.ink/v26/rounded_triangle_down.svg" width="15px"> **rounded\_triangle\_down** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/triangle_down_outline.svg" width="15px"> **triangle\_down\_outline** -> <img src="https://pinhead.ink/v26/rounded_triangle_down_outline.svg" width="15px"> **rounded\_triangle\_down\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/square.svg" width="15px"> **square** -> <img src="https://pinhead.ink/v26/rounded_square.svg" width="15px"> **rounded\_square** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/square_with_dot.svg" width="15px"> **square\_with\_dot** -> <img src="https://pinhead.ink/v26/rounded_square_with_dot.svg" width="15px"> **rounded\_square\_with\_dot** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/square_with_square_dot.svg" width="15px"> **square\_with\_square\_dot** -> <img src="https://pinhead.ink/v26/rounded_square_with_square_dot.svg" width="15px"> **rounded\_square\_with\_square\_dot** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/square_outline.svg" width="15px"> **square\_outline** -> <img src="https://pinhead.ink/v26/rounded_square_outline.svg" width="15px"> **rounded\_square\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/arrow_top_right_from_square_outline.svg" width="15px"> **arrow\_top\_right\_from\_square\_outline** -> <img src="https://pinhead.ink/v26/arrow_top_right_from_rounded_square_outline.svg" width="15px"> **arrow\_top\_right\_from\_rounded\_square\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/rectangle.svg" width="15px"> **rectangle** -> <img src="https://pinhead.ink/v26/wide_rounded_rectangle.svg" width="15px"> **wide\_rounded\_rectangle** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/rectangle_outline.svg" width="15px"> **rectangle\_outline** -> <img src="https://pinhead.ink/v26/wide_rounded_rectangle_outline.svg" width="15px"> **wide\_rounded\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v25/rectangle_tall.svg" width="15px"> **rectangle\_tall** -> <img src="https://pinhead.ink/v26/tall_rounded_rectangle.svg" width="15px"> **tall\_rounded\_rectangle** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/rectangle_tall_outline.svg" width="15px"> **rectangle\_tall\_outline** -> <img src="https://pinhead.ink/v26/tall_rounded_rectangle_outline.svg" width="15px"> **tall\_rounded\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_up_from_rectangle_outline.svg" width="15px"> **arrow\_up\_from\_rectangle\_outline** -> <img src="https://pinhead.ink/v26/arrow_up_from_wide_rectangle_outline.svg" width="15px"> **arrow\_up\_from\_wide\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_down_from_rectangle_outline.svg" width="15px"> **arrow\_down\_from\_rectangle\_outline** -> <img src="https://pinhead.ink/v26/arrow_down_from_wide_rectangle_outline.svg" width="15px"> **arrow\_down\_from\_wide\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_up_to_rectangle_outline.svg" width="15px"> **arrow\_up\_to\_rectangle\_outline** -> <img src="https://pinhead.ink/v26/arrow_up_to_wide_rectangle_outline.svg" width="15px"> **arrow\_up\_to\_wide\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_down_to_rectangle_outline.svg" width="15px"> **arrow\_down\_to\_rectangle\_outline** -> <img src="https://pinhead.ink/v26/arrow_down_to_wide_rectangle_outline.svg" width="15px"> **arrow\_down\_to\_wide\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_left_from_rectangle_tall_outline.svg" width="15px"> **arrow\_left\_from\_rectangle\_tall\_outline** -> <img src="https://pinhead.ink/v26/arrow_left_from_tall_rectangle_outline.svg" width="15px"> **arrow\_left\_from\_tall\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_right_from_rectangle_tall_outline.svg" width="15px"> **arrow\_right\_from\_rectangle\_tall\_outline** -> <img src="https://pinhead.ink/v26/arrow_right_from_tall_rectangle_outline.svg" width="15px"> **arrow\_right\_from\_tall\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_left_to_rectangle_tall_outline.svg" width="15px"> **arrow\_left\_to\_rectangle\_tall\_outline** -> <img src="https://pinhead.ink/v26/arrow_left_to_tall_rectangle_outline.svg" width="15px"> **arrow\_left\_to\_tall\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/arrow_right_to_rectangle_tall_outline.svg" width="15px"> **arrow\_right\_to\_rectangle\_tall\_outline** -> <img src="https://pinhead.ink/v26/arrow_right_to_tall_rectangle_outline.svg" width="15px"> **arrow\_right\_to\_tall\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v25/quay.svg" width="15px"> **quay** -> <img src="https://pinhead.ink/v26/tall_rectangle_beside_waters.svg" width="15px"> **tall\_rectangle\_beside\_waters** by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))

### Renamed icons (221)

* <img src="https://pinhead.ink/v26/skateboard_profile.svg" width="15px"> **skateboard** -> **skateboard\_profile**
* <img src="https://pinhead.ink/v26/spoon_beside_fork.svg" width="15px"> **spoon\_and\_fork** -> **spoon\_beside\_fork**
* <img src="https://pinhead.ink/v26/spoon_beside_chopsticks.svg" width="15px"> **spoon\_and\_chopsticks** -> **spoon\_beside\_chopsticks**
* <img src="https://pinhead.ink/v26/fork_beside_sausage.svg" width="15px"> **fork\_and\_sausage** -> **fork\_beside\_sausage**
* <img src="https://pinhead.ink/v26/fork_beside_spoon.svg" width="15px"> **fork\_and\_spoon** -> **fork\_beside\_spoon**
* <img src="https://pinhead.ink/v26/table_knife.svg" width="15px"> **knife** -> **table\_knife**
* <img src="https://pinhead.ink/v26/fork_beside_table_knife.svg" width="15px"> **fork\_and\_knife** -> **fork\_beside\_table\_knife**
* <img src="https://pinhead.ink/v26/fork_crossing_table_knife.svg" width="15px"> **fork\_crossing\_knife** -> **fork\_crossing\_table\_knife**
* <img src="https://pinhead.ink/v26/pixel_fork_beside_table_knife.svg" width="15px"> **pixel\_fork\_and\_knife** -> **pixel\_fork\_beside\_table\_knife**
* <img src="https://pinhead.ink/v26/airport_terminal_with_plane_ascending.svg" width="15px"> **airport\_terminal\_with\_plane\_takeoff** -> **airport\_terminal\_with\_plane\_ascending** ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane_ascending.svg" width="15px"> **seaplane\_takeoff** -> **seaplane\_ascending** ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/conifer_tree_beside_oval_broadleaved_tree.svg" width="15px"> **conifer\_tree\_and\_oval\_broadleaved\_tree** -> **conifer\_tree\_beside\_oval\_broadleaved\_tree**
* <img src="https://pinhead.ink/v26/person_hanging_from_pull_up_bar.svg" width="15px"> **person\_hanging\_from\_horizontal\_bar** -> **person\_hanging\_from\_pull\_up\_bar**
* <img src="https://pinhead.ink/v26/person_standing_aiming_archery_bow.svg" width="15px"> **person\_aiming\_archery\_bow** -> **person\_standing\_aiming\_archery\_bow**
* <img src="https://pinhead.ink/v26/person_slipping_on_cliff.svg" width="15px"> **person\_slipping\_down\_cliff** -> **person\_slipping\_on\_cliff**
* <img src="https://pinhead.ink/v26/person_slipping_on_cliff_into_water.svg" width="15px"> **person\_slipping\_down\_cliff\_into\_water** -> **person\_slipping\_on\_cliff\_into\_water**
* <img src="https://pinhead.ink/v26/person_slipping_on_ramp.svg" width="15px"> **person\_slipping\_down\_ramp** -> **person\_slipping\_on\_ramp**
* <img src="https://pinhead.ink/v26/person_slipping_on_steps.svg" width="15px"> **person\_slipping\_down\_steps** -> **person\_slipping\_on\_steps**
* <img src="https://pinhead.ink/v26/person_sliding_on_cliff.svg" width="15px"> **person\_sliding\_down\_cliff** -> **person\_sliding\_on\_cliff**
* <img src="https://pinhead.ink/v26/person_sliding_on_cliff_into_water.svg" width="15px"> **person\_sliding\_down\_cliff\_into\_water** -> **person\_sliding\_on\_cliff\_into\_water**
* <img src="https://pinhead.ink/v26/capsule_pill.svg" width="15px"> **pill** -> **capsule\_pill**
* <img src="https://pinhead.ink/v26/ice_uppercase.svg" width="15px"> **ice\_text** -> **ice\_uppercase** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/ice_uppercase_above_icicles.svg" width="15px"> **ice\_text\_above\_icicles** -> **ice\_uppercase\_above\_icicles** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/sos_uppercase.svg" width="15px"> **sos\_text** -> **sos\_uppercase** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/phone_down_above_sos_uppercase.svg" width="15px"> **phone\_down\_above\_sos\_text** -> **phone\_down\_above\_sos\_uppercase** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/atm_uppercase.svg" width="15px"> **atm\_text** -> **atm\_uppercase** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/art_uppercase.svg" width="15px"> **art\_text** -> **art\_uppercase** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/art_uppercase_above_swash_line.svg" width="15px"> **art\_text\_above\_swash\_line** -> **art\_uppercase\_above\_swash\_line** ([#439](https://github.com/waysidemapping/pinhead/issues/439))
* <img src="https://pinhead.ink/v26/campsite_above_canoe.svg" width="15px"> **campsite\_with\_canoe** -> **campsite\_above\_canoe**
* <img src="https://pinhead.ink/v26/person_wearing_helmet_paddling_raft_on_water.svg" width="15px"> **person\_wearing\_helmet\_padding\_raft\_on\_water** -> **person\_wearing\_helmet\_paddling\_raft\_on\_water**
* <img src="https://pinhead.ink/v26/hand_reaching_down_to_rough_surface.svg" width="15px"> **hand\_reaching\_down\_toward\_rough\_surface** -> **hand\_reaching\_down\_to\_rough\_surface**
* <img src="https://pinhead.ink/v26/two_people_above_car.svg" width="15px"> **people\_above\_car** -> **two\_people\_above\_car**
* <img src="https://pinhead.ink/v26/conifer_tree_and_flower_and_snowcapped_mountain.svg" width="15px"> **conifer\_tree\_and\_flower\_and\_mountain\_snowcapped** -> **conifer\_tree\_and\_flower\_and\_snowcapped\_mountain**
* <img src="https://pinhead.ink/v26/car_under_checkmark.svg" width="15px"> **car\_with\_checkmark** -> **car\_under\_checkmark**
* <img src="https://pinhead.ink/v26/car_under_taxi_checkerboard.svg" width="15px"> **car\_with\_taxi\_checkerboard** -> **car\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/bicycle_under_taxi_checkerboard.svg" width="15px"> **bicycle\_and\_taxi\_checkerboard** -> **bicycle\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/cargobike_under_taxi_checkerboard.svg" width="15px"> **cargobike\_and\_taxi\_checkerboard** -> **cargobike\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/motorcycle_under_taxi_checkerboard.svg" width="15px"> **motorcycle\_and\_taxi\_checkerboard** -> **motorcycle\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/motorboat_under_taxi_checkerboard.svg" width="15px"> **motorboat\_and\_taxi\_checkerboard** -> **motorboat\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/canoe_under_taxi_checkerboard.svg" width="15px"> **canoe\_and\_taxi\_checkerboard** -> **canoe\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/taxi_under_taxi_checkerboard.svg" width="15px"> **taxi\_and\_taxi\_checkerboard** -> **taxi\_under\_taxi\_checkerboard**
* <img src="https://pinhead.ink/v26/car_under_key.svg" width="15px"> **car\_and\_key** -> **car\_under\_key**
* <img src="https://pinhead.ink/v26/bicycle_under_key.svg" width="15px"> **bicycle\_and\_key** -> **bicycle\_under\_key**
* <img src="https://pinhead.ink/v26/cargobike_under_key.svg" width="15px"> **cargobike\_and\_key** -> **cargobike\_under\_key**
* <img src="https://pinhead.ink/v26/motorcycle_under_key.svg" width="15px"> **motorcycle\_and\_key** -> **motorcycle\_under\_key**
* <img src="https://pinhead.ink/v26/motorboat_under_key.svg" width="15px"> **motorboat\_and\_key** -> **motorboat\_under\_key**
* <img src="https://pinhead.ink/v26/canoe_under_key.svg" width="15px"> **canoe\_and\_key** -> **canoe\_under\_key**
* <img src="https://pinhead.ink/v26/garage_under_key.svg" width="15px"> **garage\_and\_key** -> **garage\_under\_key**
* <img src="https://pinhead.ink/v26/suitcase_under_key.svg" width="15px"> **suitcase\_and\_key** -> **suitcase\_under\_key**
* <img src="https://pinhead.ink/v26/suitcase_in_rectangle_outline_under_key.svg" width="15px"> **suitcase\_in\_rectangle\_outline\_and\_key** -> **suitcase\_in\_rectangle\_outline\_under\_key**
* <img src="https://pinhead.ink/v26/car_under_wrench.svg" width="15px"> **car\_and\_wrench** -> **car\_under\_wrench**
* <img src="https://pinhead.ink/v26/bicycle_under_wrench.svg" width="15px"> **bicycle\_and\_wrench** -> **bicycle\_under\_wrench**
* <img src="https://pinhead.ink/v26/cargobike_under_wrench.svg" width="15px"> **cargobike\_and\_wrench** -> **cargobike\_under\_wrench**
* <img src="https://pinhead.ink/v26/motorcycle_under_wrench.svg" width="15px"> **motorcycle\_and\_wrench** -> **motorcycle\_under\_wrench**
* <img src="https://pinhead.ink/v26/motorboat_under_wrench.svg" width="15px"> **motorboat\_and\_wrench** -> **motorboat\_under\_wrench**
* <img src="https://pinhead.ink/v26/garage_under_wrench.svg" width="15px"> **garage\_and\_wrench** -> **garage\_under\_wrench**
* <img src="https://pinhead.ink/v26/hearing_accessibility_symbol.svg" width="15px"> **ear\_atop\_slash** -> **hearing\_accessibility\_symbol**
* <img src="https://pinhead.ink/v26/hearing_accessibility_symbol_with_t.svg" width="15px"> **ear\_atop\_slash\_with\_t** -> **hearing\_accessibility\_symbol\_with\_t**
* <img src="https://pinhead.ink/v26/bent_tobacco_pipe.svg" width="15px"> **pipe** -> **bent\_tobacco\_pipe**
* <img src="https://pinhead.ink/v26/amphora.svg" width="15px"> **grecian\_vase** -> **amphora**
* <img src="https://pinhead.ink/v26/table_lamp.svg" width="15px"> **desk\_lamp** -> **table\_lamp**
* <img src="https://pinhead.ink/v26/bowling_pin_top_right.svg" width="15px"> **bowling\_pin** -> **bowling\_pin\_top\_right**
* <img src="https://pinhead.ink/v26/0.svg" width="15px"> **zero** -> **0** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/0_above_water.svg" width="15px"> **zero\_above\_water** -> **0\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1.svg" width="15px"> **one** -> **1** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1_above_water.svg" width="15px"> **one\_above\_water** -> **1\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1_minus.svg" width="15px"> **one\_minus** -> **1\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1_minus_above_water.svg" width="15px"> **one\_minus\_above\_water** -> **1\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1_plus.svg" width="15px"> **one\_plus** -> **1\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/1_plus_above_water.svg" width="15px"> **one\_plus\_above\_water** -> **1\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2.svg" width="15px"> **two** -> **2** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2_above_water.svg" width="15px"> **two\_above\_water** -> **2\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2_minus.svg" width="15px"> **two\_minus** -> **2\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2_minus_above_water.svg" width="15px"> **two\_minus\_above\_water** -> **2\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2_plus.svg" width="15px"> **two\_plus** -> **2\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/2_plus_above_water.svg" width="15px"> **two\_plus\_above\_water** -> **2\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3.svg" width="15px"> **three** -> **3** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3_above_water.svg" width="15px"> **three\_above\_water** -> **3\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3_minus.svg" width="15px"> **three\_minus** -> **3\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3_minus_above_water.svg" width="15px"> **three\_minus\_above\_water** -> **3\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3_plus.svg" width="15px"> **three\_plus** -> **3\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/3_plus_above_water.svg" width="15px"> **three\_plus\_above\_water** -> **3\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4.svg" width="15px"> **four** -> **4** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4_above_water.svg" width="15px"> **four\_above\_water** -> **4\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4_minus.svg" width="15px"> **four\_minus** -> **4\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4_minus_above_water.svg" width="15px"> **four\_minus\_above\_water** -> **4\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4_plus.svg" width="15px"> **four\_plus** -> **4\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/4_plus_above_water.svg" width="15px"> **four\_plus\_above\_water** -> **4\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5.svg" width="15px"> **five** -> **5** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5_above_water.svg" width="15px"> **five\_above\_water** -> **5\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5_minus.svg" width="15px"> **five\_minus** -> **5\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5_minus_above_water.svg" width="15px"> **five\_minus\_above\_water** -> **5\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5_plus.svg" width="15px"> **five\_plus** -> **5\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/5_plus_above_water.svg" width="15px"> **five\_plus\_above\_water** -> **5\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6.svg" width="15px"> **six** -> **6** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6_above_water.svg" width="15px"> **six\_above\_water** -> **6\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6_minus.svg" width="15px"> **six\_minus** -> **6\_minus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6_minus_above_water.svg" width="15px"> **six\_minus\_above\_water** -> **6\_minus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6_plus.svg" width="15px"> **six\_plus** -> **6\_plus** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/6_plus_above_water.svg" width="15px"> **six\_plus\_above\_water** -> **6\_plus\_above\_water** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/7.svg" width="15px"> **seven** -> **7** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/8.svg" width="15px"> **eight** -> **8** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/9.svg" width="15px"> **nine** -> **9** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/10.svg" width="15px"> **ten** -> **10** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/11.svg" width="15px"> **eleven** -> **11** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/12.svg" width="15px"> **twelve** -> **12** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_111.svg" width="15px"> **phone\_down\_above\_one\_one\_one** -> **phone\_down\_above\_111** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_112.svg" width="15px"> **phone\_down\_above\_one\_one\_two** -> **phone\_down\_above\_112** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_123.svg" width="15px"> **phone\_down\_above\_one\_two\_three** -> **phone\_down\_above\_123** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_211.svg" width="15px"> **phone\_down\_above\_two\_one\_one** -> **phone\_down\_above\_211** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_311.svg" width="15px"> **phone\_down\_above\_three\_one\_one** -> **phone\_down\_above\_311** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_411.svg" width="15px"> **phone\_down\_above\_four\_one\_one** -> **phone\_down\_above\_411** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_511.svg" width="15px"> **phone\_down\_above\_five\_one\_one** -> **phone\_down\_above\_511** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_611.svg" width="15px"> **phone\_down\_above\_six\_one\_one** -> **phone\_down\_above\_611** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_711.svg" width="15px"> **phone\_down\_above\_seven\_one\_one** -> **phone\_down\_above\_711** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_811.svg" width="15px"> **phone\_down\_above\_eight\_one\_one** -> **phone\_down\_above\_811** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_911.svg" width="15px"> **phone\_down\_above\_nine\_one\_one** -> **phone\_down\_above\_911** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_988.svg" width="15px"> **phone\_down\_above\_nine\_eight\_eight** -> **phone\_down\_above\_988** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/phone_down_above_999.svg" width="15px"> **phone\_down\_above\_nine\_nine\_nine** -> **phone\_down\_above\_999** ([#307](https://github.com/waysidemapping/pinhead/issues/307))
* <img src="https://pinhead.ink/v26/bagel_with_seeds.svg" width="15px"> **bagel\_seeded** -> **bagel\_with\_seeds**
* <img src="https://pinhead.ink/v26/step_ladder_double_sided.svg" width="15px"> **step\_ladder\_doubled\_sided** -> **step\_ladder\_double\_sided**
* <img src="https://pinhead.ink/v26/three_stacked_books.svg" width="15px"> **three\_books\_stacked** -> **three\_stacked\_books**
* <img src="https://pinhead.ink/v26/person_diving_wearing_scuba_gear.svg" width="15px"> **person\_wearing\_scuba\_gear\_diving** -> **person\_diving\_wearing\_scuba\_gear**
* <img src="https://pinhead.ink/v26/person_diving_wearing_scuba_gear_under_water.svg" width="15px"> **person\_wearing\_scuba\_gear\_diving\_under\_water** -> **person\_diving\_wearing\_scuba\_gear\_under\_water**
* <img src="https://pinhead.ink/v26/person_scrambling_on_cliff_wearing_backpack.svg" width="15px"> **person\_wearing\_backpack\_scrambling\_up\_cliff** -> **person\_scrambling\_on\_cliff\_wearing\_backpack**
* <img src="https://pinhead.ink/v26/person_walking_with_hiking_pole_wearing_backpack_in_gable_roofed_shelter.svg" width="15px"> **person\_wearing\_backpack\_walking\_with\_hiking\_pole\_in\_gable\_roofed\_shelter** -> **person\_walking\_with\_hiking\_pole\_wearing\_backpack\_in\_gable\_roofed\_shelter**
* <img src="https://pinhead.ink/v26/person_walking_with_hiking_pole_wearing_backpack.svg" width="15px"> **person\_wearing\_backpack\_walking\_with\_hiking\_pole** -> **person\_walking\_with\_hiking\_pole\_wearing\_backpack**
* <img src="https://pinhead.ink/v26/person_crouching_wearing_backpack_and_headlamp.svg" width="15px"> **person\_wearing\_backpack\_and\_headlamp\_crouching** -> **person\_crouching\_wearing\_backpack\_and\_headlamp**
* <img src="https://pinhead.ink/v26/person_walking_with_bicycle.svg" width="15px"> **person\_walking\_bicycle** -> **person\_walking\_with\_bicycle**
* <img src="https://pinhead.ink/v26/person_front_kicking_wearing_martial_arts_belt.svg" width="15px"> **person\_wearing\_martial\_arts\_belt\_front\_kicking** -> **person\_front\_kicking\_wearing\_martial\_arts\_belt**
* <img src="https://pinhead.ink/v26/person_racing_bicycle.svg" width="15px"> **person\_bicycle\_racing** -> **person\_racing\_bicycle**
* <img src="https://pinhead.ink/v26/person_swinging_racket_at_ball.svg" width="15px"> **person\_playing\_tennis** -> **person\_swinging\_racket\_at\_ball**
* <img src="https://pinhead.ink/v26/people_running.svg" width="15px"> **person\_running\_after\_person** -> **people\_running**
* <img src="https://pinhead.ink/v26/person_holding_baseball_bat.svg" width="15px"> **person\_baseball\_batting** -> **person\_holding\_baseball\_bat**
* <img src="https://pinhead.ink/v26/person_swinging_cricket_bat_at_ball.svg" width="15px"> **person\_cricket\_batting\_at\_cricket\_ball** -> **person\_swinging\_cricket\_bat\_at\_ball**
* <img src="https://pinhead.ink/v26/person_jockeying_horse_running.svg" width="15px"> **person\_jockeying\_racehorse** -> **person\_jockeying\_horse\_running**
* <img src="https://pinhead.ink/v26/person_kneeling_praying.svg" width="15px"> **person\_kneeling\_and\_praying** -> **person\_kneeling\_praying**
* <img src="https://pinhead.ink/v26/person_running_kicking_ball.svg" width="15px"> **person\_playing\_soccer** -> **person\_running\_kicking\_ball**
* <img src="https://pinhead.ink/v26/person_spiking_ball.svg" width="15px"> **person\_spiking\_volleyball** -> **person\_spiking\_ball**
* <img src="https://pinhead.ink/v26/person.svg" width="15px"> **head\_and\_shoulders** -> **person**
* <img src="https://pinhead.ink/v26/pixel_person.svg" width="15px"> **pixel\_head\_and\_shoulders** -> **pixel\_person**
* <img src="https://pinhead.ink/v26/two_people_standing_beside_person_standing_pointing.svg" width="15px"> **people\_and\_person\_pointing** -> **two\_people\_standing\_beside\_person\_standing\_pointing**
* <img src="https://pinhead.ink/v26/overweight_person_standing.svg" width="15px"> **overweight\_person** -> **overweight\_person\_standing**
* <img src="https://pinhead.ink/v26/underweight_person_standing.svg" width="15px"> **underweight\_person** -> **underweight\_person\_standing**
* <img src="https://pinhead.ink/v26/pregnant_person_standing.svg" width="15px"> **pregnant\_person** -> **pregnant\_person\_standing**
* <img src="https://pinhead.ink/v26/person_carrying_shopping_bags.svg" width="15px"> **person\_holding\_shopping\_bags\_walking** -> **person\_carrying\_shopping\_bags**
* <img src="https://pinhead.ink/v26/person_standing_holding_branches.svg" width="15px"> **person\_holding\_branches** -> **person\_standing\_holding\_branches**
* <img src="https://pinhead.ink/v26/person_standing_in_water_wearing_swim_briefs_holding_bucket.svg" width="15px"> **person\_in\_water\_wearing\_swim\_briefs\_holding\_bucket** -> **person\_standing\_in\_water\_wearing\_swim\_briefs\_holding\_bucket**
* <img src="https://pinhead.ink/v26/person_standing_holding_cane.svg" width="15px"> **person\_holding\_cane** -> **person\_standing\_holding\_cane**
* <img src="https://pinhead.ink/v26/person_standing_wearing_dress_holding_cane.svg" width="15px"> **person\_wearing\_dress\_holding\_cane** -> **person\_standing\_wearing\_dress\_holding\_cane**
* <img src="https://pinhead.ink/v26/person_standing_wearing_cowboy_hat_holding_coiled_rope.svg" width="15px"> **person\_wearing\_cowboy\_hat\_holding\_coiled\_rope** -> **person\_standing\_wearing\_cowboy\_hat\_holding\_coiled\_rope**
* <img src="https://pinhead.ink/v26/person_squatting_beside_person_standing_reaching_up.svg" width="15px"> **person\_squatting\_and\_person\_reaching\_up** -> **person\_squatting\_beside\_person\_standing\_reaching\_up**
* <img src="https://pinhead.ink/v26/person_racing_jetski_in_waves.svg" width="15px"> **person\_boat\_racing\_in\_waves** -> **person\_racing\_jetski\_in\_waves**
* <img src="https://pinhead.ink/v26/person_sitting_on_swing.svg" width="15px"> **person\_on\_swing** -> **person\_sitting\_on\_swing**
* <img src="https://pinhead.ink/v26/person_riding_swing.svg" width="15px"> **person\_on\_inclined\_swing** -> **person\_riding\_swing**
* <img src="https://pinhead.ink/v26/plane_top_right_and_plane_bottom_left.svg" width="15px"> **planes\_bidirectional** -> **plane\_top\_right\_and\_plane\_bottom\_left**
* <img src="https://pinhead.ink/v26/waters_meeting_shore.svg" width="15px"> **shore** -> **waters\_meeting\_shore**
* <img src="https://pinhead.ink/v26/steam_train_with_smiling_face.svg" width="15px"> **kids\_train** -> **steam\_train\_with\_smiling\_face**
* <img src="https://pinhead.ink/v26/steam_train_with_smiling_face_with_tires.svg" width="15px"> **kids\_train\_with\_tires** -> **steam\_train\_with\_smiling\_face\_with\_tires**
* <img src="https://pinhead.ink/v26/steam_train_with_smiling_face_on_railway_track.svg" width="15px"> **kids\_train\_on\_railway\_track** -> **steam\_train\_with\_smiling\_face\_on\_railway\_track**
* <img src="https://pinhead.ink/v26/person_boarding_steam_train_with_smiling_face_on_railway_track.svg" width="15px"> **person\_boarding\_kids\_train\_on\_railway\_track** -> **person\_boarding\_steam\_train\_with\_smiling\_face\_on\_railway\_track**
* <img src="https://pinhead.ink/v26/racket.svg" width="15px"> **racquet** -> **racket**
* <img src="https://pinhead.ink/v26/barred_door.svg" width="15px"> **jail\_door** -> **barred\_door**
* <img src="https://pinhead.ink/v26/three_dots_left_right.svg" width="15px"> **three\_dot\_horizontal\_line** -> **three\_dots\_left\_right**
* <img src="https://pinhead.ink/v26/three_dots_left_right_in_wide_rounded_rectangle.svg" width="15px"> **three\_dot\_horizontal\_line\_in\_rectangle** -> **three\_dots\_left\_right\_in\_wide\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/two_dots_left_right_in_wide_rounded_rectangle.svg" width="15px"> **two\_dot\_horizontal\_line\_in\_rectangle** -> **two\_dots\_left\_right\_in\_wide\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/three_dots_up_down.svg" width="15px"> **three\_dot\_vertical\_line** -> **three\_dots\_up\_down**
* <img src="https://pinhead.ink/v26/three_dots_up_down_in_tall_rounded_rectangle.svg" width="15px"> **three\_dot\_vertical\_line\_in\_rectangle** -> **three\_dots\_up\_down\_in\_tall\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/two_dots_up_down_in_tall_rounded_rectangle.svg" width="15px"> **two\_dot\_vertical\_line\_in\_rectangle** -> **two\_dots\_up\_down\_in\_tall\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/eighth_notes.svg" width="15px"> **music\_notes\_eighth** -> **eighth\_notes**
* <img src="https://pinhead.ink/v26/sixteenth_notes.svg" width="15px"> **music\_notes\_sixteenth** -> **sixteenth\_notes**
* <img src="https://pinhead.ink/v26/quarter_note_with_optical_disc.svg" width="15px"> **music\_note\_with\_optical\_disc** -> **quarter\_note\_with\_optical\_disc**
* <img src="https://pinhead.ink/v26/palette_with_quarter_note.svg" width="15px"> **palette\_with\_music\_note** -> **palette\_with\_quarter\_note**
* <img src="https://pinhead.ink/v26/book_with_eighth_notes.svg" width="15px"> **book\_with\_music\_notes\_eighth** -> **book\_with\_eighth\_notes**
* <img src="https://pinhead.ink/v26/horse_spring_rider.svg" width="15px"> **spring\_rider** -> **horse\_spring\_rider**
* <img src="https://pinhead.ink/v26/cable_railway_track.svg" width="15px"> **railway\_cable\_track** -> **cable\_railway\_track** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/miniature_railway_track.svg" width="15px"> **railway\_track\_mini** -> **miniature\_railway\_track** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/narrow_railway_track.svg" width="15px"> **railway\_track\_narrow\_gauge** -> **narrow\_railway\_track** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/spiky_fish_under_x.svg" width="15px"> **spiky\_fish\_with\_x** -> **spiky\_fish\_under\_x**
* <img src="https://pinhead.ink/v26/american_sign_language_interpretation.svg" width="15px"> **hands\_sign\_language\_interpretation** -> **american\_sign\_language\_interpretation**
* <img src="https://pinhead.ink/v26/fish_jumping_above_cascade.svg" width="15px"> **fish\_jumping\_up\_cascade** -> **fish\_jumping\_above\_cascade**
* <img src="https://pinhead.ink/v26/flagstick_with_pennant_in_hole_on_golf_green.svg" width="15px"> **golf\_green** -> **flagstick\_with\_pennant\_in\_hole\_on\_golf\_green**
* <img src="https://pinhead.ink/v26/checkered_flag_on_flag_handle.svg" width="15px"> **flag\_checkered** -> **checkered\_flag\_on\_flag\_handle**
* <img src="https://pinhead.ink/v26/flag_on_flag_handle_above_railway_track.svg" width="15px"> **flag\_above\_railway\_track** -> **flag\_on\_flag\_handle\_above\_railway\_track**
* <img src="https://pinhead.ink/v26/crossed_chopsticks.svg" width="15px"> **chopsticks\_crossed** -> **crossed\_chopsticks**
* <img src="https://pinhead.ink/v26/tall_gate.svg" width="15px"> **gate\_tall** -> **tall\_gate** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_plus.svg" width="15px"> **plus\_squat** -> **wide\_plus** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_winding_way.svg" width="15px"> **winding\_way\_wide** -> **wide\_winding\_way** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/narrow_winding_way.svg" width="15px"> **winding\_way\_narrow** -> **narrow\_winding\_way** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p.svg" width="15px"> **p\_wide** -> **wide\_p** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p_in_parking_structure.svg" width="15px"> **p\_wide\_in\_parking\_structure** -> **wide\_p\_in\_parking\_structure** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p_on_parking_line.svg" width="15px"> **p\_wide\_on\_parking\_line** -> **wide\_p\_on\_parking\_line** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p_under_roof.svg" width="15px"> **p\_wide\_under\_roof** -> **wide\_p\_under\_roof** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p_with_bicycle.svg" width="15px"> **p\_wide\_with\_bicycle** -> **wide\_p\_with\_bicycle** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_p_with_parking_meter.svg" width="15px"> **p\_wide\_with\_parking\_meter** -> **wide\_p\_with\_parking\_meter** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/parking_stall_markings_with_wide_p.svg" width="15px"> **parking\_stall\_markings\_with\_p\_wide** -> **parking\_stall\_markings\_with\_wide\_p** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e.svg" width="15px"> **e\_wide** -> **wide\_e** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e_in_parking_structure.svg" width="15px"> **e\_wide\_in\_parking\_structure** -> **wide\_e\_in\_parking\_structure** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e_on_parking_line.svg" width="15px"> **e\_wide\_on\_parking\_line** -> **wide\_e\_on\_parking\_line** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e_under_roof.svg" width="15px"> **e\_wide\_under\_roof** -> **wide\_e\_under\_roof** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e_with_bicycle.svg" width="15px"> **e\_wide\_with\_bicycle** -> **wide\_e\_with\_bicycle** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/wide_e_with_parking_meter.svg" width="15px"> **e\_wide\_with\_parking\_meter** -> **wide\_e\_with\_parking\_meter** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/parking_stall_markings_with_wide_e.svg" width="15px"> **parking\_stall\_markings\_with\_e\_wide** -> **parking\_stall\_markings\_with\_wide\_e** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/circle_with_horizontal_bar.svg" width="15px"> **no\_entry** -> **circle\_with\_horizontal\_bar**
* <img src="https://pinhead.ink/v26/wide_rounded_triangle_down.svg" width="15px"> **triangle\_down\_squat** -> **wide\_rounded\_triangle\_down** ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/ethernet_port_in_rounded_square.svg" width="15px"> **ethernet\_port\_in\_square** -> **ethernet\_port\_in\_rounded\_square** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangles_left_right_in_wide_rounded_rectangle.svg" width="15px"> **triangles\_left\_right\_in\_rectangle** -> **triangles\_left\_right\_in\_wide\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangles_left_right_in_wide_rounded_rectangle_outline.svg" width="15px"> **triangles\_left\_right\_in\_rectangle\_outline** -> **triangles\_left\_right\_in\_wide\_rounded\_rectangle\_outline** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangles_up_down_in_tall_rounded_rectangle.svg" width="15px"> **triangles\_up\_down\_in\_rectangle** -> **triangles\_up\_down\_in\_tall\_rounded\_rectangle** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangles_up_down_in_tall_rounded_rectangle_outline.svg" width="15px"> **triangles\_up\_down\_in\_rectangle\_outline** -> **triangles\_up\_down\_in\_tall\_rounded\_rectangle\_outline** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/rounded_diamond.svg" width="15px"> **diamond** -> **rounded\_diamond** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/rounded_diamond_outline.svg" width="15px"> **diamond\_outline** -> **rounded\_diamond\_outline** ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/tall_rounded_diamond.svg" width="15px"> **diamond\_tall** -> **tall\_rounded\_diamond** ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_rounded_diamond_outline.svg" width="15px"> **diamond\_tall\_outline** -> **tall\_rounded\_diamond\_outline** ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_rounded_double_diamond.svg" width="15px"> **double\_diamond\_tall** -> **tall\_rounded\_double\_diamond** ([#451](https://github.com/waysidemapping/pinhead/issues/451), [#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_isosceles_trapezoid_down.svg" width="15px"> **isosceles\_trapezoid\_tall\_down** -> **tall\_isosceles\_trapezoid\_down** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_isosceles_trapezoid_up.svg" width="15px"> **isosceles\_trapezoid\_tall\_up** -> **tall\_isosceles\_trapezoid\_up** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_parallelogram_left.svg" width="15px"> **parallelogram\_tall\_left** -> **tall\_parallelogram\_left** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_parallelogram_right.svg" width="15px"> **parallelogram\_tall\_right** -> **tall\_parallelogram\_right** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_chevron_up.svg" width="15px"> **chevron\_up\_tall** -> **tall\_chevron\_up** ([#463](https://github.com/waysidemapping/pinhead/issues/463))
* <img src="https://pinhead.ink/v26/tall_chevron_up_outline.svg" width="15px"> **chevron\_up\_tall\_outline** -> **tall\_chevron\_up\_outline** ([#463](https://github.com/waysidemapping/pinhead/issues/463))

### Merged icons (1)

* <img src="https://pinhead.ink/v25/gumdrop_head_and_shoulders.svg" width="15px"> **gumdrop\_head\_and\_shoulders** -> <img src="https://pinhead.ink/v26/person.svg" width="15px"> **person**

### Redesigned icons (148)

* <img src="https://pinhead.ink/v25/stone_wall.svg" width="15px"> -> <img src="https://pinhead.ink/v26/stone_wall.svg" width="15px"> **stone\_wall** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/bowling_ball.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bowling_ball.svg" width="15px"> **bowling\_ball** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/soccer_ball.svg" width="15px"> -> <img src="https://pinhead.ink/v26/soccer_ball.svg" width="15px"> **soccer\_ball** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/basketball_in_basketball_net.svg" width="15px"> -> <img src="https://pinhead.ink/v26/basketball_in_basketball_net.svg" width="15px"> **basketball\_in\_basketball\_net** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/rolled_paper_in_bottle.svg" width="15px"> -> <img src="https://pinhead.ink/v26/rolled_paper_in_bottle.svg" width="15px"> **rolled\_paper\_in\_bottle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/japanese_teacup_with_steam.svg" width="15px"> -> <img src="https://pinhead.ink/v26/japanese_teacup_with_steam.svg" width="15px"> **japanese\_teacup\_with\_steam** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/coffee_mug_with_steam.svg" width="15px"> -> <img src="https://pinhead.ink/v26/coffee_mug_with_steam.svg" width="15px"> **coffee\_mug\_with\_steam** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/lattice_tower_with_ball_tip_antenna_on_ground_with_beams.svg" width="15px"> -> <img src="https://pinhead.ink/v26/lattice_tower_with_ball_tip_antenna_on_ground_with_beams.svg" width="15px"> **lattice\_tower\_with\_ball\_tip\_antenna\_on\_ground\_with\_beams** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/lattice_tower_with_observation_deck_on_ground.svg" width="15px"> -> <img src="https://pinhead.ink/v26/lattice_tower_with_observation_deck_on_ground.svg" width="15px"> **lattice\_tower\_with\_observation\_deck\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/skyscraper_on_ground.svg" width="15px"> -> <img src="https://pinhead.ink/v26/skyscraper_on_ground.svg" width="15px"> **skyscraper\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/lowrise_apartment_building_on_ground.svg" width="15px"> -> <img src="https://pinhead.ink/v26/lowrise_apartment_building_on_ground.svg" width="15px"> **lowrise\_apartment\_building\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/floor_lamp.svg" width="15px"> -> <img src="https://pinhead.ink/v26/floor_lamp.svg" width="15px"> **floor\_lamp** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/potted_flower.svg" width="15px"> -> <img src="https://pinhead.ink/v26/potted_flower.svg" width="15px"> **potted\_flower** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/palm_tree.svg" width="15px"> -> <img src="https://pinhead.ink/v26/palm_tree.svg" width="15px"> **palm\_tree** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/coconut_palm_tree_on_hill_in_water.svg" width="15px"> -> <img src="https://pinhead.ink/v26/coconut_palm_tree_on_hill_in_water.svg" width="15px"> **coconut\_palm\_tree\_on\_hill\_in\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/squat_rock.svg" width="15px"> -> <img src="https://pinhead.ink/v26/squat_rock.svg" width="15px"> **squat\_rock** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/person_standing.svg" width="15px"> -> <img src="https://pinhead.ink/v26/person_standing.svg" width="15px"> **person\_standing** by [@quincylvania](https://github.com/quincylvania) ([#448](https://github.com/waysidemapping/pinhead/issues/448))
* <img src="https://pinhead.ink/v25/ahimsa_hand_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/ahimsa_hand_outline.svg" width="15px"> **ahimsa\_hand\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/memorial_stone_with_latin_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/memorial_stone_with_latin_cross.svg" width="15px"> **memorial\_stone\_with\_latin\_cross** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/coffin_with_latin_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/coffin_with_latin_cross.svg" width="15px"> **coffin\_with\_latin\_cross** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/greek_cross.svg" width="15px"> **greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/heart_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/heart_with_greek_cross.svg" width="15px"> **heart\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/pawprint.svg" width="15px"> -> <img src="https://pinhead.ink/v26/pawprint.svg" width="15px"> **pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/pawprint_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/pawprint_with_greek_cross.svg" width="15px"> **pawprint\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/bag_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bag_with_greek_cross.svg" width="15px"> **bag\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/mountain_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/mountain_with_greek_cross.svg" width="15px"> **mountain\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/compact_box_truck_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/compact_box_truck_with_greek_cross.svg" width="15px"> **compact\_box\_truck\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/pill_bottle_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/pill_bottle_with_greek_cross.svg" width="15px"> **pill\_bottle\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/mortar_and_pestle_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/mortar_and_pestle_with_greek_cross.svg" width="15px"> **mortar\_and\_pestle\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/droplet.svg" width="15px"> **droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/droplet_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/droplet_with_greek_cross.svg" width="15px"> **droplet\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230), [#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/water_bottle.svg" width="15px"> -> <img src="https://pinhead.ink/v26/water_bottle.svg" width="15px"> **water\_bottle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/droplet_from_pipes.svg" width="15px"> -> <img src="https://pinhead.ink/v26/droplet_from_pipes.svg" width="15px"> **droplet\_from\_pipes** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/syrup_jug_and_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/syrup_jug_and_droplet.svg" width="15px"> **syrup\_jug\_and\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/syrup_jug_with_maple_leaf_and_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/syrup_jug_with_maple_leaf_and_droplet.svg" width="15px"> **syrup\_jug\_with\_maple\_leaf\_and\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/syrup_jug_with_sugarcane_stalk_with_leaves_and_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/syrup_jug_with_sugarcane_stalk_with_leaves_and_droplet.svg" width="15px"> **syrup\_jug\_with\_sugarcane\_stalk\_with\_leaves\_and\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/manhole_cover_with_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/manhole_cover_with_droplet.svg" width="15px"> **manhole\_cover\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/utility_device_with_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/utility_device_with_droplet.svg" width="15px"> **utility\_device\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/utility_meter_with_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/utility_meter_with_droplet.svg" width="15px"> **utility\_meter\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/utility_valve_with_droplet.svg" width="15px"> -> <img src="https://pinhead.ink/v26/utility_valve_with_droplet.svg" width="15px"> **utility\_valve\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#230](https://github.com/waysidemapping/pinhead/issues/230))
* <img src="https://pinhead.ink/v25/dog_sitting_and_exclamation_point.svg" width="15px"> -> <img src="https://pinhead.ink/v26/dog_sitting_and_exclamation_point.svg" width="15px"> **dog\_sitting\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/dog_sitting_wearing_collar_and_exclamation_point.svg" width="15px"> -> <img src="https://pinhead.ink/v26/dog_sitting_wearing_collar_and_exclamation_point.svg" width="15px"> **dog\_sitting\_wearing\_collar\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cat_sitting.svg" width="15px"> -> <img src="https://pinhead.ink/v26/cat_sitting.svg" width="15px"> **cat\_sitting** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/wolf_head_and_exclamation_point.svg" width="15px"> -> <img src="https://pinhead.ink/v26/wolf_head_and_exclamation_point.svg" width="15px"> **wolf\_head\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/bird.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bird.svg" width="15px"> **bird** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/sea_lion.svg" width="15px"> -> <img src="https://pinhead.ink/v26/sea_lion.svg" width="15px"> **sea\_lion** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/traffic_cone_and_exclamation_point.svg" width="15px"> -> <img src="https://pinhead.ink/v26/traffic_cone_and_exclamation_point.svg" width="15px"> **traffic\_cone\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag.svg" width="15px"> **shopping\_bag** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_baht.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_baht.svg" width="15px"> **shopping\_bag\_with\_baht** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_dollar.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_dollar.svg" width="15px"> **shopping\_bag\_with\_dollar** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_euro.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_euro.svg" width="15px"> **shopping\_bag\_with\_euro** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_peso.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_peso.svg" width="15px"> **shopping\_bag\_with\_peso** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_pound.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_pound.svg" width="15px"> **shopping\_bag\_with\_pound** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_ruble.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_ruble.svg" width="15px"> **shopping\_bag\_with\_ruble** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_rupee.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_rupee.svg" width="15px"> **shopping\_bag\_with\_rupee** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_shekel.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_shekel.svg" width="15px"> **shopping\_bag\_with\_shekel** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_yen_yuan.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_yen_yuan.svg" width="15px"> **shopping\_bag\_with\_yen\_yuan** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_ampersand.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_ampersand.svg" width="15px"> **shopping\_bag\_with\_ampersand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_anime_eye_and_eyebrow.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_anime_eye_and_eyebrow.svg" width="15px"> **shopping\_bag\_with\_anime\_eye\_and\_eyebrow** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_arrows_recirculating.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_arrows_recirculating.svg" width="15px"> **shopping\_bag\_with\_arrows\_recirculating** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_heart.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_heart.svg" width="15px"> **shopping\_bag\_with\_heart** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_pawprint.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_pawprint.svg" width="15px"> **shopping\_bag\_with\_pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/shopping_bag_with_tag.svg" width="15px"> -> <img src="https://pinhead.ink/v26/shopping_bag_with_tag.svg" width="15px"> **shopping\_bag\_with\_tag** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/suitcase.svg" width="15px"> -> <img src="https://pinhead.ink/v26/suitcase.svg" width="15px"> **suitcase** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/briefcase.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase.svg" width="15px"> **briefcase** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/briefcase_with_bolt.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase_with_bolt.svg" width="15px"> **briefcase\_with\_bolt** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/briefcase_with_greek_cross.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase_with_greek_cross.svg" width="15px"> **briefcase\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#258](https://github.com/waysidemapping/pinhead/issues/258))
* <img src="https://pinhead.ink/v25/briefcase_with_heavy_six_point_asterisk.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase_with_heavy_six_point_asterisk.svg" width="15px"> **briefcase\_with\_heavy\_six\_point\_asterisk** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/briefcase_with_shield.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase_with_shield.svg" width="15px"> **briefcase\_with\_shield** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/briefcase_with_info_i.svg" width="15px"> -> <img src="https://pinhead.ink/v26/briefcase_with_info_i.svg" width="15px"> **briefcase\_with\_info\_i** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/banknote.svg" width="15px"> -> <img src="https://pinhead.ink/v26/banknote.svg" width="15px"> **banknote** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v25/banknote_in_hand.svg" width="15px"> -> <img src="https://pinhead.ink/v26/banknote_in_hand.svg" width="15px"> **banknote\_in\_hand** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v25/banknote_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/banknote_in_slot.svg" width="15px"> **banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v25/arrow_up_to_banknote_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_banknote_in_slot.svg" width="15px"> **arrow\_up\_to\_banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v25/arrow_down_from_banknote_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_banknote_in_slot.svg" width="15px"> **arrow\_down\_from\_banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v25/person_riding_dog_sled.svg" width="15px"> -> <img src="https://pinhead.ink/v26/person_riding_dog_sled.svg" width="15px"> **person\_riding\_dog\_sled** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/sea_star.svg" width="15px"> -> <img src="https://pinhead.ink/v26/sea_star.svg" width="15px"> **sea\_star** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/bicycle_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bicycle_and_arrow_right_above_arrow_left.svg" width="15px"> **bicycle\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/cargobike_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/cargobike_and_arrow_right_above_arrow_left.svg" width="15px"> **cargobike\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/suitcase_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/suitcase_and_arrow_right_above_arrow_left.svg" width="15px"> **suitcase\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/motorcycle_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/motorcycle_and_arrow_right_above_arrow_left.svg" width="15px"> **motorcycle\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/car_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/car_and_arrow_right_above_arrow_left.svg" width="15px"> **car\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/taxi_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/taxi_and_arrow_right_above_arrow_left.svg" width="15px"> **taxi\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/motorboat_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/motorboat_and_arrow_right_above_arrow_left.svg" width="15px"> **motorboat\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/key_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/key_and_arrow_right_above_arrow_left.svg" width="15px"> **key\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/canoe_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/canoe_and_arrow_right_above_arrow_left.svg" width="15px"> **canoe\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_arrow_right_above_arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bear_spray_can_with_spray_and_arrow_right_above_arrow_left.svg" width="15px"> **bear\_spray\_can\_with\_spray\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/microscope.svg" width="15px"> -> <img src="https://pinhead.ink/v26/microscope.svg" width="15px"> **microscope** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/dumping_ash_in_bin.svg" width="15px"> -> <img src="https://pinhead.ink/v26/dumping_ash_in_bin.svg" width="15px"> **dumping\_ash\_in\_bin** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/sign_beside_car.svg" width="15px"> -> <img src="https://pinhead.ink/v26/sign_beside_car.svg" width="15px"> **sign\_beside\_car** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/sign_beside_taxi.svg" width="15px"> -> <img src="https://pinhead.ink/v26/sign_beside_taxi.svg" width="15px"> **sign\_beside\_taxi** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/sign_beside_bench_with_backrest.svg" width="15px"> -> <img src="https://pinhead.ink/v26/sign_beside_bench_with_backrest.svg" width="15px"> **sign\_beside\_bench\_with\_backrest** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/bench_with_backrest_in_rectangular_shelter.svg" width="15px"> -> <img src="https://pinhead.ink/v26/bench_with_backrest_in_rectangular_shelter.svg" width="15px"> **bench\_with\_backrest\_in\_rectangular\_shelter** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/propane_tank_with_gas_flame.svg" width="15px"> -> <img src="https://pinhead.ink/v26/propane_tank_with_gas_flame.svg" width="15px"> **propane\_tank\_with\_gas\_flame** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/deer_with_antlers.svg" width="15px"> -> <img src="https://pinhead.ink/v26/deer_with_antlers.svg" width="15px"> **deer\_with\_antlers** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/pickleball_paddle_with_ball.svg" width="15px"> -> <img src="https://pinhead.ink/v26/pickleball_paddle_with_ball.svg" width="15px"> **pickleball\_paddle\_with\_ball** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/table_tennis_paddle.svg" width="15px"> -> <img src="https://pinhead.ink/v26/table_tennis_paddle.svg" width="15px"> **table\_tennis\_paddle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/stomach.svg" width="15px"> -> <img src="https://pinhead.ink/v26/stomach.svg" width="15px"> **stomach** by [@quincylvania](https://github.com/quincylvania) ([#288](https://github.com/waysidemapping/pinhead/issues/288))
* <img src="https://pinhead.ink/v25/crab.svg" width="15px"> -> <img src="https://pinhead.ink/v26/crab.svg" width="15px"> **crab** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/noodle_bowl_and_chopsticks_with_noodles.svg" width="15px"> -> <img src="https://pinhead.ink/v26/noodle_bowl_and_chopsticks_with_noodles.svg" width="15px"> **noodle\_bowl\_and\_chopsticks\_with\_noodles** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/arrow_up.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up.svg" width="15px"> **arrow\_up** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down.svg" width="15px"> **arrow\_down** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_left.svg" width="15px"> **arrow\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_right.svg" width="15px"> **arrow\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_top_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_top_right.svg" width="15px"> **arrow\_top\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_bottom_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_bottom_right.svg" width="15px"> **arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_bottom_right_to_eight_point_asterisk.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_bottom_right_to_eight_point_asterisk.svg" width="15px"> **arrow\_bottom\_right\_to\_eight\_point\_asterisk** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_top_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_top_left.svg" width="15px"> **arrow\_top\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_bottom_left.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_bottom_left.svg" width="15px"> **arrow\_bottom\_left** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrows_left_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrows_left_right.svg" width="15px"> **arrows\_left\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrows_left_right_above_water.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrows_left_right_above_water.svg" width="15px"> **arrows\_left\_right\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrows_left_right_above_waters.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrows_left_right_above_waters.svg" width="15px"> **arrows\_left\_right\_above\_waters** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrows_up_down_in_left_right_brackets.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrows_up_down_in_left_right_brackets.svg" width="15px"> **arrows\_up\_down\_in\_left\_right\_brackets** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_from_down_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_from_down_bracket.svg" width="15px"> **arrow\_up\_from\_down\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_up_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_up_bracket.svg" width="15px"> **arrow\_down\_from\_up\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_left_from_right_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_left_from_right_bracket.svg" width="15px"> **arrow\_left\_from\_right\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_right_from_left_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_right_from_left_bracket.svg" width="15px"> **arrow\_right\_from\_left\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_up_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_up_bracket.svg" width="15px"> **arrow\_up\_to\_up\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_to_down_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_to_down_bracket.svg" width="15px"> **arrow\_down\_to\_down\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_left_to_left_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_left_to_left_bracket.svg" width="15px"> **arrow\_left\_to\_left\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_right_to_right_bracket.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_right_to_right_bracket.svg" width="15px"> **arrow\_right\_to\_right\_bracket** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_banknote_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_banknote_in_slot.svg" width="15px"> **arrow\_up\_to\_banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_book_with_bookmark_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_book_with_bookmark_in_slot.svg" width="15px"> **arrow\_up\_to\_book\_with\_bookmark\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_envelope_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_envelope_in_slot.svg" width="15px"> **arrow\_up\_to\_envelope\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_payment_card_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_payment_card_in_slot.svg" width="15px"> **arrow\_up\_to\_payment\_card\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_up_to_ticket_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_up_to_ticket_in_slot.svg" width="15px"> **arrow\_up\_to\_ticket\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_banknote_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_banknote_in_slot.svg" width="15px"> **arrow\_down\_from\_banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_book_with_bookmark_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_book_with_bookmark_in_slot.svg" width="15px"> **arrow\_down\_from\_book\_with\_bookmark\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_envelope_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_envelope_in_slot.svg" width="15px"> **arrow\_down\_from\_envelope\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_payment_card_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_payment_card_in_slot.svg" width="15px"> **arrow\_down\_from\_payment\_card\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/arrow_down_from_ticket_in_slot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/arrow_down_from_ticket_in_slot.svg" width="15px"> **arrow\_down\_from\_ticket\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/flush_curb_with_arrow_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/flush_curb_with_arrow_right.svg" width="15px"> **flush\_curb\_with\_arrow\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/rolled_curb_with_arrow_bottom_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/rolled_curb_with_arrow_bottom_right.svg" width="15px"> **rolled\_curb\_with\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/lowered_curb_with_arrow_bottom_right.svg" width="15px"> -> <img src="https://pinhead.ink/v26/lowered_curb_with_arrow_bottom_right.svg" width="15px"> **lowered\_curb\_with\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/raised_curb_with_arrow_down.svg" width="15px"> -> <img src="https://pinhead.ink/v26/raised_curb_with_arrow_down.svg" width="15px"> **raised\_curb\_with\_arrow\_down** by [@quincylvania](https://github.com/quincylvania) ([#337](https://github.com/waysidemapping/pinhead/issues/337))
* <img src="https://pinhead.ink/v25/dot_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/dot_outline.svg" width="15px"> **dot\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle.svg" width="15px"> **circle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_with_dot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_with_dot.svg" width="15px"> **circle\_with\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_with_dot_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_with_dot_outline.svg" width="15px"> **circle\_with\_dot\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_outline.svg" width="15px"> **circle\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_outline_with_star.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_outline_with_star.svg" width="15px"> **circle\_outline\_with\_star** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_outline_with_top_left_quarter_and_bottom_right_quarter.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_outline_with_top_left_quarter_and_bottom_right_quarter.svg" width="15px"> **circle\_outline\_with\_top\_left\_quarter\_and\_bottom\_right\_quarter** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_outline_with_dot.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_outline_with_dot.svg" width="15px"> **circle\_outline\_with\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_outline_with_dot_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_outline_with_dot_outline.svg" width="15px"> **circle\_outline\_with\_dot\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/circle_with_fallout_shelter_symbol.svg" width="15px"> -> <img src="https://pinhead.ink/v26/circle_with_fallout_shelter_symbol.svg" width="15px"> **circle\_with\_fallout\_shelter\_symbol** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/cairn.svg" width="15px"> -> <img src="https://pinhead.ink/v26/cairn.svg" width="15px"> **cairn** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/octagon.svg" width="15px"> -> <img src="https://pinhead.ink/v26/octagon.svg" width="15px"> **octagon** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v25/octagon_outline.svg" width="15px"> -> <img src="https://pinhead.ink/v26/octagon_outline.svg" width="15px"> **octagon\_outline** by [@quincylvania](https://github.com/quincylvania)

### Added icons (430)

* <img src="https://pinhead.ink/v26/fountain_from_ground.svg" width="15px"> Add **fountain\_from\_ground** by [@Geo-2695](https://github.com/Geo-2695) ([#256](https://github.com/waysidemapping/pinhead/issues/256))
* <img src="https://pinhead.ink/v26/bento.svg" width="15px"> Add **bento** by [@ooosssay](https://github.com/ooosssay) ([#426](https://github.com/waysidemapping/pinhead/issues/426), [#352](https://github.com/waysidemapping/pinhead/issues/352))
* <img src="https://pinhead.ink/v26/food_truck.svg" width="15px"> Add **food\_truck** by [@ooosssay](https://github.com/ooosssay) ([#429](https://github.com/waysidemapping/pinhead/issues/429), [#92](https://github.com/waysidemapping/pinhead/issues/92))
* <img src="https://pinhead.ink/v26/tree_trunk_with_plaque.svg" width="15px"> Add **tree\_trunk\_with\_plaque** by [@ooosssay](https://github.com/ooosssay) ([#474](https://github.com/waysidemapping/pinhead/issues/474), [#253](https://github.com/waysidemapping/pinhead/issues/253))
* <img src="https://pinhead.ink/v26/tree_trunk.svg" width="15px"> Add **tree\_trunk** by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pencil_beside_ruler.svg" width="15px"> Add **pencil\_beside\_ruler** by [@ooosssay](https://github.com/ooosssay) ([#475](https://github.com/waysidemapping/pinhead/issues/475))
* <img src="https://pinhead.ink/v26/spray_paint_can.svg" width="15px"> Add **spray\_paint\_can** by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#427](https://github.com/waysidemapping/pinhead/issues/427), [#246](https://github.com/waysidemapping/pinhead/issues/246))
* <img src="https://pinhead.ink/v26/spray_paint_can_with_spray.svg" width="15px"> Add **spray\_paint\_can\_with\_spray** by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#427](https://github.com/waysidemapping/pinhead/issues/427), [#246](https://github.com/waysidemapping/pinhead/issues/246))
* <img src="https://pinhead.ink/v26/wall_with_battlement.svg" width="15px"> Add **wall\_with\_battlement** by [@Geo-2695](https://github.com/Geo-2695), [@quincylvania](https://github.com/quincylvania) ([#457](https://github.com/waysidemapping/pinhead/issues/457))
* <img src="https://pinhead.ink/v26/stone_wall_with_battlement.svg" width="15px"> Add **stone\_wall\_with\_battlement** by [@Geo-2695](https://github.com/Geo-2695), [@quincylvania](https://github.com/quincylvania) ([#456](https://github.com/waysidemapping/pinhead/issues/456))
* <img src="https://pinhead.ink/v26/stone_wall_with_battlement_and_sallyport.svg" width="15px"> Add **stone\_wall\_with\_battlement\_and\_sallyport** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/brick_wall.svg" width="15px"> Add **brick\_wall** by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#428](https://github.com/waysidemapping/pinhead/issues/428))
* <img src="https://pinhead.ink/v26/brick_wall_with_bolt.svg" width="15px"> Add **brick\_wall\_with\_bolt** by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#428](https://github.com/waysidemapping/pinhead/issues/428))
* <img src="https://pinhead.ink/v26/brick_wall_with_battlement.svg" width="15px"> Add **brick\_wall\_with\_battlement** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/brick_wall_with_battlement_and_sallyport.svg" width="15px"> Add **brick\_wall\_with\_battlement\_and\_sallyport** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/curling_stone.svg" width="15px"> Add **curling\_stone** by [@ooosssay](https://github.com/ooosssay) ([#331](https://github.com/waysidemapping/pinhead/issues/331))
* <img src="https://pinhead.ink/v26/tennis_ball.svg" width="15px"> Add **tennis\_ball** by [@wmisener](https://github.com/wmisener), [@quincylvania](https://github.com/quincylvania) ([#4](https://github.com/waysidemapping/pinhead/issues/4))
* <img src="https://pinhead.ink/v26/baseball.svg" width="15px"> Add **baseball** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/skateboard.svg" width="15px"> Add **skateboard** by [@wmisener](https://github.com/wmisener) from [OSM Americana](https://github.com/osm-americana/openstreetmap-americana) imported by [@quincylvania](https://github.com/quincylvania) ([#4](https://github.com/waysidemapping/pinhead/issues/4))
* <img src="https://pinhead.ink/v26/skateboard_deck.svg" width="15px"> Add **skateboard\_deck** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/basketball.svg" width="15px"> Add **basketball** by [@wmisener](https://github.com/wmisener), [@quincylvania](https://github.com/quincylvania) ([#4](https://github.com/waysidemapping/pinhead/issues/4))
* <img src="https://pinhead.ink/v26/horse.svg" width="15px"> Add **horse** by [@quincylvania](https://github.com/quincylvania) ([#12](https://github.com/waysidemapping/pinhead/issues/12))
* <img src="https://pinhead.ink/v26/horse_running.svg" width="15px"> Add **horse\_running** by [@quincylvania](https://github.com/quincylvania) ([#12](https://github.com/waysidemapping/pinhead/issues/12))
* <img src="https://pinhead.ink/v26/horse_high_stepping.svg" width="15px"> Add **horse\_high\_stepping** by [@wmisener](https://github.com/wmisener) from [OSM Americana](https://github.com/osm-americana/openstreetmap-americana) imported by [@quincylvania](https://github.com/quincylvania) ([#4](https://github.com/waysidemapping/pinhead/issues/4), [#12](https://github.com/waysidemapping/pinhead/issues/12))
* <img src="https://pinhead.ink/v26/kick_scooter.svg" width="15px"> Add **kick\_scooter** by [@qugebert](https://github.com/qugebert), [@quincylvania](https://github.com/quincylvania) ([#482](https://github.com/waysidemapping/pinhead/issues/482))
* <img src="https://pinhead.ink/v26/kick_scooter_with_power_cord.svg" width="15px"> Add **kick\_scooter\_with\_power\_cord** from [source](https://upload.wikimedia.org/wikipedia/commons/4/44/Zusatzzeichen_1010-68_-_Elektrokleinstfahrzeuge_im_Sinne_der_Elektrokleinstfahrzeuge-Verordnung_%28eKFV%29%2C_%28450x600%29%2C_StVO_2020.svg) imported by [@qugebert](https://github.com/qugebert), [@quincylvania](https://github.com/quincylvania) ([#482](https://github.com/waysidemapping/pinhead/issues/482))
* <img src="https://pinhead.ink/v26/phone_top_right_and_exclamation_point.svg" width="15px"> Add **phone\_top\_right\_and\_exclamation\_point** by [@Geo-2695](https://github.com/Geo-2695), [@quincylvania](https://github.com/quincylvania) ([#470](https://github.com/waysidemapping/pinhead/issues/470))
* <img src="https://pinhead.ink/v26/phone_top_right_and_question_mark.svg" width="15px"> Add **phone\_top\_right\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/phone_top_right_and_minus.svg" width="15px"> Add **phone\_top\_right\_and\_minus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/phone_bottom_right_and_minus.svg" width="15px"> Add **phone\_bottom\_right\_and\_minus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/phone_right_beside_droplet.svg" width="15px"> Add **phone\_right\_beside\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/phone_right_beside_gas_flame.svg" width="15px"> Add **phone\_right\_beside\_gas\_flame** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/spoon_beside_table_knife.svg" width="15px"> Add **spoon\_beside\_table\_knife** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/fork_beside_plate_beside_table_knife.svg" width="15px"> Add **fork\_beside\_plate\_beside\_table\_knife** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/fork_beside_fish.svg" width="15px"> Add **fork\_beside\_fish** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/fish_beside_sausage.svg" width="15px"> Add **fish\_beside\_sausage** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/loaf_of_bread_above_fish.svg" width="15px"> Add **loaf\_of\_bread\_above\_fish** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/spiky_fish_under_fillet_knife.svg" width="15px"> Add **spiky\_fish\_under\_fillet\_knife** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bridge_shape_bottom_left_top_right.svg" width="15px"> Add **bridge\_shape\_bottom\_left\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bridge_shape_left_right.svg" width="15px"> Add **bridge\_shape\_left\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bridge_shape_up_down.svg" width="15px"> Add **bridge\_shape\_up\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bridge_in_water.svg" width="15px"> Add **bridge\_in\_water** by [@quincylvania](https://github.com/quincylvania) ([#290](https://github.com/waysidemapping/pinhead/issues/290))
* <img src="https://pinhead.ink/v26/funnel.svg" width="15px"> Add **funnel** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/stardust.svg" width="15px"> Add **stardust** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/tangram_square.svg" width="15px"> Add **tangram\_square** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/map_pin_with_dot_on_open_book.svg" width="15px"> Add **map\_pin\_with\_dot\_on\_open\_book** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/crossed_bones.svg" width="15px"> Add **crossed\_bones** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/japanese_teacup.svg" width="15px"> Add **japanese\_teacup** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/japanese_teacup_and_wifi.svg" width="15px"> Add **japanese\_teacup\_and\_wifi** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/japanese_teacup_and_pawprint.svg" width="15px"> Add **japanese\_teacup\_and\_pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/handled_teacup.svg" width="15px"> Add **handled\_teacup** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/handled_teacup_and_saucer_with_steam.svg" width="15px"> Add **handled\_teacup\_and\_saucer\_with\_steam** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/handled_teacup_with_steam.svg" width="15px"> Add **handled\_teacup\_with\_steam** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffee_mug.svg" width="15px"> Add **coffee\_mug** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffee_mug_and_saucer.svg" width="15px"> Add **coffee\_mug\_and\_saucer** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffee_mug_and_wifi.svg" width="15px"> Add **coffee\_mug\_and\_wifi** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffee_mug_and_pawprint.svg" width="15px"> Add **coffee\_mug\_and\_pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/car_beside_bench_on_ground.svg" width="15px"> Add **car\_beside\_bench\_on\_ground** by [@ooosssay](https://github.com/ooosssay) ([#473](https://github.com/waysidemapping/pinhead/issues/473))
* <img src="https://pinhead.ink/v26/lattice_tower_with_ball_tip_antenna_on_ground.svg" width="15px"> Add **lattice\_tower\_with\_ball\_tip\_antenna\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/lattice_tower_with_observation_deck.svg" width="15px"> Add **lattice\_tower\_with\_observation\_deck** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/skyscraper.svg" width="15px"> Add **skyscraper** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/lowrise_apartment_building.svg" width="15px"> Add **lowrise\_apartment\_building** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/plane_ascending.svg" width="15px"> Add **plane\_ascending** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_ascending_above_water.svg" width="15px"> Add **plane\_ascending\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_cruising.svg" width="15px"> Add **plane\_cruising** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_cruising_above_ground.svg" width="15px"> Add **plane\_cruising\_above\_ground** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_cruising_above_water.svg" width="15px"> Add **plane\_cruising\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_descending.svg" width="15px"> Add **plane\_descending** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_descending_above_ground.svg" width="15px"> Add **plane\_descending\_above\_ground** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/plane_descending_above_water.svg" width="15px"> Add **plane\_descending\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane.svg" width="15px"> Add **seaplane** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane_above_water.svg" width="15px"> Add **seaplane\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane_on_water.svg" width="15px"> Add **seaplane\_on\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane_descending.svg" width="15px"> Add **seaplane\_descending** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/seaplane_descending_above_water.svg" width="15px"> Add **seaplane\_descending\_above\_water** by [@quincylvania](https://github.com/quincylvania) ([#236](https://github.com/waysidemapping/pinhead/issues/236))
* <img src="https://pinhead.ink/v26/conifer_tree_beside_oval_broadleaved_tree_on_ground.svg" width="15px"> Add **conifer\_tree\_beside\_oval\_broadleaved\_tree\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/conifer_tree_beside_conifer_tree_on_ground.svg" width="15px"> Add **conifer\_tree\_beside\_conifer\_tree\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/oval_broadleaved_tree_beside_oval_broadleaved_tree_on_ground.svg" width="15px"> Add **oval\_broadleaved\_tree\_beside\_oval\_broadleaved\_tree\_on\_ground** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pull_up_bar.svg" width="15px"> Add **pull\_up\_bar** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/floor_lamp_beside_potted_flower.svg" width="15px"> Add **floor\_lamp\_beside\_potted\_flower** by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
* <img src="https://pinhead.ink/v26/coconut_palm_tree_on_hill.svg" width="15px"> Add **coconut\_palm\_tree\_on\_hill** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/squat_rock_with_inscription.svg" width="15px"> Add **squat\_rock\_with\_inscription** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_standing_with_heart.svg" width="15px"> Add **person\_standing\_with\_heart** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rectangle_outline_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **rectangle\_outline\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_people_standing_in_rectangle_outline_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **two\_people\_standing\_in\_rectangle\_outline\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/crates_in_rectangle_outline_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **crates\_in\_rectangle\_outline\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rectangle_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **rectangle\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_standing_in_rectangle_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **person\_standing\_in\_rectangle\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_people_standing_in_rectangle_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **two\_people\_standing\_in\_rectangle\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_people_standing_in_rectangle_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **three\_people\_standing\_in\_rectangle\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/crates_in_rectangle_under_arrow_up_beside_arrow_down.svg" width="15px"> Add **crates\_in\_rectangle\_under\_arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_aiming_archery_bow.svg" width="15px"> Add **person\_aiming\_archery\_bow** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_sitting_in_seat_beside_person_sitting_in_seat.svg" width="15px"> Add **person\_sitting\_in\_seat\_beside\_person\_sitting\_in\_seat** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_sitting_on_lifeguard_stand.svg" width="15px"> Add **person\_sitting\_on\_lifeguard\_stand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_diving.svg" width="15px"> Add **person\_diving** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_falling.svg" width="15px"> Add **person\_falling** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_slipping.svg" width="15px"> Add **person\_slipping** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_sliding.svg" width="15px"> Add **person\_sliding** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/ahimsa_hand.svg" width="15px"> Add **ahimsa\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/angel_moroni_on_square.svg" width="15px"> Add **angel\_moroni\_on\_square** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/ahimsa_hand_on_square.svg" width="15px"> Add **ahimsa\_hand\_on\_square** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/ankh_on_square.svg" width="15px"> Add **ankh\_on\_square** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/nine_point_star_outline_on_square.svg" width="15px"> Add **nine\_point\_star\_outline\_on\_square** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/question_mark_on_square.svg" width="15px"> Add **question\_mark\_on\_square** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/exclamation_point_on_square.svg" width="15px"> Add **exclamation\_point\_on\_square** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/memorial_stone_with_star_and_crescent.svg" width="15px"> Add **memorial\_stone\_with\_star\_and\_crescent** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_star_of_david.svg" width="15px"> Add **memorial\_stone\_with\_star\_of\_david** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_om.svg" width="15px"> Add **memorial\_stone\_with\_om** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_yin_yang.svg" width="15px"> Add **memorial\_stone\_with\_yin\_yang** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_khanda.svg" width="15px"> Add **memorial\_stone\_with\_khanda** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_dharma_wheel.svg" width="15px"> Add **memorial\_stone\_with\_dharma\_wheel** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_quaker_star.svg" width="15px"> Add **memorial\_stone\_with\_quaker\_star** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_flaming_chalice.svg" width="15px"> Add **memorial\_stone\_with\_flaming\_chalice** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_angel_moroni.svg" width="15px"> Add **memorial\_stone\_with\_angel\_moroni** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_ahimsa_hand.svg" width="15px"> Add **memorial\_stone\_with\_ahimsa\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_ankh.svg" width="15px"> Add **memorial\_stone\_with\_ankh** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_nine_point_star_outline.svg" width="15px"> Add **memorial\_stone\_with\_nine\_point\_star\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/memorial_stone_with_question_mark.svg" width="15px"> Add **memorial\_stone\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/memorial_stone_with_exclamation_point.svg" width="15px"> Add **memorial\_stone\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/coffin_with_star_and_crescent.svg" width="15px"> Add **coffin\_with\_star\_and\_crescent** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_star_of_david.svg" width="15px"> Add **coffin\_with\_star\_of\_david** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_om.svg" width="15px"> Add **coffin\_with\_om** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_yin_yang.svg" width="15px"> Add **coffin\_with\_yin\_yang** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_khanda.svg" width="15px"> Add **coffin\_with\_khanda** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_dharma_wheel.svg" width="15px"> Add **coffin\_with\_dharma\_wheel** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_quaker_star.svg" width="15px"> Add **coffin\_with\_quaker\_star** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_flaming_chalice.svg" width="15px"> Add **coffin\_with\_flaming\_chalice** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_angel_moroni.svg" width="15px"> Add **coffin\_with\_angel\_moroni** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_ahimsa_hand.svg" width="15px"> Add **coffin\_with\_ahimsa\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_ankh.svg" width="15px"> Add **coffin\_with\_ankh** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_nine_point_star_outline.svg" width="15px"> Add **coffin\_with\_nine\_point\_star\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/coffin_with_question_mark.svg" width="15px"> Add **coffin\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/coffin_with_exclamation_point.svg" width="15px"> Add **coffin\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/circular_pill.svg" width="15px"> Add **circular\_pill** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/two_circular_pills.svg" width="15px"> Add **two\_circular\_pills** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/three_circular_pills.svg" width="15px"> Add **three\_circular\_pills** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/four_circular_pills.svg" width="15px"> Add **four\_circular\_pills** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/rx_symbol.svg" width="15px"> Add **rx\_symbol** by [@quincylvania](https://github.com/quincylvania) ([#299](https://github.com/waysidemapping/pinhead/issues/299))
* <img src="https://pinhead.ink/v26/capsule_pill_and_rx_symbol.svg" width="15px"> Add **capsule\_pill\_and\_rx\_symbol** by [@quincylvania](https://github.com/quincylvania) ([#299](https://github.com/waysidemapping/pinhead/issues/299))
* <img src="https://pinhead.ink/v26/circular_pill_and_capsule_pill.svg" width="15px"> Add **circular\_pill\_and\_capsule\_pill** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangular_pill_and_circular_pill_and_capsule_pill.svg" width="15px"> Add **triangular\_pill\_and\_circular\_pill\_and\_capsule\_pill** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/greek_cross_outline.svg" width="15px"> Add **greek\_cross\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pill_bottle.svg" width="15px"> Add **pill\_bottle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pill_bottle_with_rx_symbol.svg" width="15px"> Add **pill\_bottle\_with\_rx\_symbol** by [@quincylvania](https://github.com/quincylvania) ([#299](https://github.com/waysidemapping/pinhead/issues/299))
* <img src="https://pinhead.ink/v26/pill_bottle_with_circular_pill.svg" width="15px"> Add **pill\_bottle\_with\_circular\_pill** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pill_bottle_with_capsule_pill.svg" width="15px"> Add **pill\_bottle\_with\_capsule\_pill** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/mortar_and_pestle.svg" width="15px"> Add **mortar\_and\_pestle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/mortar_and_pestle_with_rx_symbol.svg" width="15px"> Add **mortar\_and\_pestle\_with\_rx\_symbol** by [@quincylvania](https://github.com/quincylvania) ([#299](https://github.com/waysidemapping/pinhead/issues/299))
* <img src="https://pinhead.ink/v26/book_with_greek_cross.svg" width="15px"> Add **book\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/book_with_heavy_six_point_asterisk.svg" width="15px"> Add **book\_with\_heavy\_six\_point\_asterisk** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/medal_ribbon_with_greek_cross.svg" width="15px"> Add **medal\_ribbon\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/medal_ribbon_with_circle.svg" width="15px"> Add **medal\_ribbon\_with\_circle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_with_shine.svg" width="15px"> Add **droplet\_with\_shine** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_outline.svg" width="15px"> Add **droplet\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_with_question_mark.svg" width="15px"> Add **droplet\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/droplet_with_exclamation_point.svg" width="15px"> Add **droplet\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/droplet_and_greek_cross.svg" width="15px"> Add **droplet\_and\_greek\_cross** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_and_question_mark.svg" width="15px"> Add **droplet\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/droplet_and_exclamation_point.svg" width="15px"> Add **droplet\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/droplet_above_water.svg" width="15px"> Add **droplet\_above\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/water_bottle_and_droplet.svg" width="15px"> Add **water\_bottle\_and\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bucket_with_droplet.svg" width="15px"> Add **bucket\_with\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/gasoline_pump_with_droplet.svg" width="15px"> Add **gasoline\_pump\_with\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/gasoline_pump_with_question_mark.svg" width="15px"> Add **gasoline\_pump\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/gasoline_pump_with_exclamation_point.svg" width="15px"> Add **gasoline\_pump\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/globe_gasoline_pump_with_droplet.svg" width="15px"> Add **globe\_gasoline\_pump\_with\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_under_roof.svg" width="15px"> Add **droplet\_under\_roof** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_in_gable_roofed_shelter.svg" width="15px"> Add **droplet\_in\_gable\_roofed\_shelter** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/slide_and_droplet.svg" width="15px"> Add **slide\_and\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/syrup_jug_with_droplet.svg" width="15px"> Add **syrup\_jug\_with\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sitting_tank_toilet_with_droplet.svg" width="15px"> Add **sitting\_tank\_toilet\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#39](https://github.com/waysidemapping/pinhead/issues/39), [#182](https://github.com/waysidemapping/pinhead/issues/182))
* <img src="https://pinhead.ink/v26/dog_sitting_wearing_collar_and_droplet.svg" width="15px"> Add **dog\_sitting\_wearing\_collar\_and\_droplet** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cat_sitting_and_whistle.svg" width="15px"> Add **cat\_sitting\_and\_whistle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cat_sitting_and_question_mark.svg" width="15px"> Add **cat\_sitting\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cat_sitting_and_exclamation_point.svg" width="15px"> Add **cat\_sitting\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/dog_sitting_and_question_mark.svg" width="15px"> Add **dog\_sitting\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/dog_sitting_wearing_collar_and_question_mark.svg" width="15px"> Add **dog\_sitting\_wearing\_collar\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/wolf_head_and_question_mark.svg" width="15px"> Add **wolf\_head\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/gull_and_question_mark.svg" width="15px"> Add **gull\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/hairy_caterpillar_and_question_mark.svg" width="15px"> Add **hairy\_caterpillar\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/bird_and_question_mark.svg" width="15px"> Add **bird\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bird_and_exclamation_point.svg" width="15px"> Add **bird\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sea_lion_and_whistle.svg" width="15px"> Add **sea\_lion\_and\_whistle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sea_lion_and_question_mark.svg" width="15px"> Add **sea\_lion\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sea_lion_and_exclamation_point.svg" width="15px"> Add **sea\_lion\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/lion_and_whistle.svg" width="15px"> Add **lion\_and\_whistle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/lion_and_question_mark.svg" width="15px"> Add **lion\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/lion_and_exclamation_point.svg" width="15px"> Add **lion\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bear_and_question_mark.svg" width="15px"> Add **bear\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bear_and_exclamation_point.svg" width="15px"> Add **bear\_and\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/flush_curb_with_exclamation_point.svg" width="15px"> Add **flush\_curb\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/lowered_curb_with_exclamation_point.svg" width="15px"> Add **lowered\_curb\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/rolled_curb_with_exclamation_point.svg" width="15px"> Add **rolled\_curb\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/raised_curb_with_exclamation_point.svg" width="15px"> Add **raised\_curb\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/traffic_cone_and_question_mark.svg" width="15px"> Add **traffic\_cone\_and\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/phone_right_beside_question_mark.svg" width="15px"> Add **phone\_right\_beside\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/spherical_virus_with_question_mark.svg" width="15px"> Add **spherical\_virus\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/badge_shield_with_question_mark.svg" width="15px"> Add **badge\_shield\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/badge_shield_with_exclamation_point.svg" width="15px"> Add **badge\_shield\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/badge_shield_with_wifi.svg" width="15px"> Add **badge\_shield\_with\_wifi** by [@quincylvania](https://github.com/quincylvania) ([#47](https://github.com/waysidemapping/pinhead/issues/47))
* <img src="https://pinhead.ink/v26/shopping_bag_with_droplet.svg" width="15px"> Add **shopping\_bag\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_gas_flame.svg" width="15px"> Add **shopping\_bag\_with\_gas\_flame** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_open_book.svg" width="15px"> Add **shopping\_bag\_with\_open\_book** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_rocketship.svg" width="15px"> Add **shopping\_bag\_with\_rocketship** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_stardust.svg" width="15px"> Add **shopping\_bag\_with\_stardust** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_map_pin_with_dot.svg" width="15px"> Add **shopping\_bag\_with\_map\_pin\_with\_dot** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_wifi.svg" width="15px"> Add **shopping\_bag\_with\_wifi** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_greek_cross.svg" width="15px"> Add **shopping\_bag\_with\_greek\_cross** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_heavy_six_point_asterisk.svg" width="15px"> Add **shopping\_bag\_with\_heavy\_six\_point\_asterisk** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_circular_pill_and_capsule_pill.svg" width="15px"> Add **shopping\_bag\_with\_circular\_pill\_and\_capsule\_pill** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_rx_symbol.svg" width="15px"> Add **shopping\_bag\_with\_rx\_symbol** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_apple.svg" width="15px"> Add **shopping\_bag\_with\_apple** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_crab.svg" width="15px"> Add **shopping\_bag\_with\_crab** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_leaf.svg" width="15px"> Add **shopping\_bag\_with\_leaf** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_conifer_tree.svg" width="15px"> Add **shopping\_bag\_with\_conifer\_tree** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_shield.svg" width="15px"> Add **shopping\_bag\_with\_shield** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_eighth_notes.svg" width="15px"> Add **shopping\_bag\_with\_eighth\_notes** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_venus.svg" width="15px"> Add **shopping\_bag\_with\_venus** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_mars.svg" width="15px"> Add **shopping\_bag\_with\_mars** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365), [#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/shopping_bag_with_venus_mars.svg" width="15px"> Add **shopping\_bag\_with\_venus\_mars** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365), [#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/shopping_bag_with_info_i.svg" width="15px"> Add **shopping\_bag\_with\_info\_i** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365))
* <img src="https://pinhead.ink/v26/shopping_bag_with_question_mark.svg" width="15px"> Add **shopping\_bag\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365), [#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/shopping_bag_with_exclamation_point.svg" width="15px"> Add **shopping\_bag\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#365](https://github.com/waysidemapping/pinhead/issues/365), [#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/briefcase_with_phone_top_right.svg" width="15px"> Add **briefcase\_with\_phone\_top\_right** by [@quincylvania](https://github.com/quincylvania) ([#477](https://github.com/waysidemapping/pinhead/issues/477))
* <img src="https://pinhead.ink/v26/briefcase_with_heart.svg" width="15px"> Add **briefcase\_with\_heart** by [@quincylvania](https://github.com/quincylvania) ([#343](https://github.com/waysidemapping/pinhead/issues/343))
* <img src="https://pinhead.ink/v26/briefcase_with_droplet.svg" width="15px"> Add **briefcase\_with\_droplet** by [@quincylvania](https://github.com/quincylvania) ([#237](https://github.com/waysidemapping/pinhead/issues/237))
* <img src="https://pinhead.ink/v26/briefcase_with_gas_flame.svg" width="15px"> Add **briefcase\_with\_gas\_flame** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_open_book.svg" width="15px"> Add **briefcase\_with\_open\_book** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_rx_symbol.svg" width="15px"> Add **briefcase\_with\_rx\_symbol** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_circular_pill_and_capsule_pill.svg" width="15px"> Add **briefcase\_with\_circular\_pill\_and\_capsule\_pill** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_leaf.svg" width="15px"> Add **briefcase\_with\_leaf** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_conifer_tree.svg" width="15px"> Add **briefcase\_with\_conifer\_tree** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_pawprint.svg" width="15px"> Add **briefcase\_with\_pawprint** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_apple.svg" width="15px"> Add **briefcase\_with\_apple** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_stardust.svg" width="15px"> Add **briefcase\_with\_stardust** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_megaphone.svg" width="15px"> Add **briefcase\_with\_megaphone** by [@quincylvania](https://github.com/quincylvania) ([#359](https://github.com/waysidemapping/pinhead/issues/359))
* <img src="https://pinhead.ink/v26/briefcase_with_venus.svg" width="15px"> Add **briefcase\_with\_venus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_mars.svg" width="15px"> Add **briefcase\_with\_mars** by [@quincylvania](https://github.com/quincylvania) ([#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/briefcase_with_venus_mars.svg" width="15px"> Add **briefcase\_with\_venus\_mars** by [@quincylvania](https://github.com/quincylvania) ([#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/briefcase_with_wifi.svg" width="15px"> Add **briefcase\_with\_wifi** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_map_pin_with_dot.svg" width="15px"> Add **briefcase\_with\_map\_pin\_with\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_eighth_notes.svg" width="15px"> Add **briefcase\_with\_eighth\_notes** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/briefcase_with_question_mark.svg" width="15px"> Add **briefcase\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/briefcase_with_exclamation_point.svg" width="15px"> Add **briefcase\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/vending_machine_with_question_mark.svg" width="15px"> Add **vending\_machine\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/vending_machine_with_exclamation_point.svg" width="15px"> Add **vending\_machine\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/vending_machine_with_mars.svg" width="15px"> Add **vending\_machine\_with\_mars** by [@quincylvania](https://github.com/quincylvania) ([#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/vending_machine_with_venus_mars.svg" width="15px"> Add **vending\_machine\_with\_venus\_mars** by [@quincylvania](https://github.com/quincylvania) ([#391](https://github.com/waysidemapping/pinhead/issues/391))
* <img src="https://pinhead.ink/v26/book_with_question_mark.svg" width="15px"> Add **book\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/book_with_exclamation_point.svg" width="15px"> Add **book\_with\_exclamation\_point** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/outstretched_hand.svg" width="15px"> Add **outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/droplet_above_outstretched_hand.svg" width="15px"> Add **droplet\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/gas_flame_above_outstretched_hand.svg" width="15px"> Add **gas\_flame\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/greek_cross_above_outstretched_hand.svg" width="15px"> Add **greek\_cross\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/heavy_six_point_asterisk_above_outstretched_hand.svg" width="15px"> Add **heavy\_six\_point\_asterisk\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rx_symbol_above_outstretched_hand.svg" width="15px"> Add **rx\_symbol\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania) ([#299](https://github.com/waysidemapping/pinhead/issues/299))
* <img src="https://pinhead.ink/v26/circular_pill_and_capsule_pill_above_outstretched_hand.svg" width="15px"> Add **circular\_pill\_and\_capsule\_pill\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/leaf_above_outstretched_hand.svg" width="15px"> Add **leaf\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/conifer_tree_above_outstretched_hand.svg" width="15px"> Add **conifer\_tree\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/stardust_above_outstretched_hand.svg" width="15px"> Add **stardust\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/apple_above_outstretched_hand.svg" width="15px"> Add **apple\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/loaf_of_bread_above_outstretched_hand.svg" width="15px"> Add **loaf\_of\_bread\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/open_book_above_outstretched_hand.svg" width="15px"> Add **open\_book\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/dove_above_outstretched_hand.svg" width="15px"> Add **dove\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/wifi_above_outstretched_hand.svg" width="15px"> Add **wifi\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/map_pin_with_dot_above_outstretched_hand.svg" width="15px"> Add **map\_pin\_with\_dot\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/question_mark_above_outstretched_hand.svg" width="15px"> Add **question\_mark\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/exclamation_point_above_outstretched_hand.svg" width="15px"> Add **exclamation\_point\_above\_outstretched\_hand** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/three_stacked_banknotes_in_slot.svg" width="15px"> Add **three\_stacked\_banknotes\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v26/three_stacked_banknotes.svg" width="15px"> Add **three\_stacked\_banknotes** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v26/arrow_up_to_three_stacked_banknotes_in_slot.svg" width="15px"> Add **arrow\_up\_to\_three\_stacked\_banknotes\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v26/arrow_down_from_three_stacked_banknotes_in_slot.svg" width="15px"> Add **arrow\_down\_from\_three\_stacked\_banknotes\_in\_slot** by [@quincylvania](https://github.com/quincylvania) ([#310](https://github.com/waysidemapping/pinhead/issues/310))
* <img src="https://pinhead.ink/v26/atm_uppercase_above_banknote_in_slot.svg" width="15px"> Add **atm\_uppercase\_above\_banknote\_in\_slot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/thumbs_down_hand_with_sleeve.svg" width="15px"> Add **thumbs\_down\_hand\_with\_sleeve** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/tourboat.svg" width="15px"> Add **tourboat** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/airboat.svg" width="15px"> Add **airboat** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/canoe_under_wrench.svg" width="15px"> Add **canoe\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/canoe_above_water.svg" width="15px"> Add **canoe\_above\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/person_wearing_helmet_paddling_raft.svg" width="15px"> Add **person\_wearing\_helmet\_paddling\_raft** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_dogs.svg" width="15px"> Add **three\_dogs** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_dogs_wearing_collars.svg" width="15px"> Add **three\_dogs\_wearing\_collars** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_dogs_under_dog_sled.svg" width="15px"> Add **three\_dogs\_under\_dog\_sled** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_dogs_wearing_collars_under_dog_sled.svg" width="15px"> Add **three\_dogs\_wearing\_collars\_under\_dog\_sled** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/dog_sled.svg" width="15px"> Add **dog\_sled** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/hand_reaching_down_to_water.svg" width="15px"> Add **hand\_reaching\_down\_to\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sea_star_under_water.svg" width="15px"> Add **sea\_star\_under\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_under_wrench.svg" width="15px"> Add **sedan\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_with_raised_hood_under_wrench.svg" width="15px"> Add **sedan\_with\_raised\_hood\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_under_key.svg" width="15px"> Add **sedan\_under\_key** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_and_arrow_right_above_arrow_left.svg" width="15px"> Add **sedan\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_under_taxi_checkerboard.svg" width="15px"> Add **sedan\_under\_taxi\_checkerboard** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_and_locked_lock_with_keyhole.svg" width="15px"> Add **sedan\_and\_locked\_lock\_with\_keyhole** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sedan_under_list_beside_checkmark.svg" width="15px"> Add **sedan\_under\_list\_beside\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_people_above_sedan.svg" width="15px"> Add **two\_people\_above\_sedan** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_under_wrench.svg" width="15px"> Add **station\_wagon\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_with_raised_hood_under_wrench.svg" width="15px"> Add **station\_wagon\_with\_raised\_hood\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_under_key.svg" width="15px"> Add **station\_wagon\_under\_key** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_and_arrow_right_above_arrow_left.svg" width="15px"> Add **station\_wagon\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_under_taxi_checkerboard.svg" width="15px"> Add **station\_wagon\_under\_taxi\_checkerboard** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_and_locked_lock_with_keyhole.svg" width="15px"> Add **station\_wagon\_and\_locked\_lock\_with\_keyhole** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/station_wagon_under_list_beside_checkmark.svg" width="15px"> Add **station\_wagon\_under\_list\_beside\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_people_above_station_wagon.svg" width="15px"> Add **two\_people\_above\_station\_wagon** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_under_wrench.svg" width="15px"> Add **pickup\_truck\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_with_raised_hood_under_wrench.svg" width="15px"> Add **pickup\_truck\_with\_raised\_hood\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_under_key.svg" width="15px"> Add **pickup\_truck\_under\_key** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_and_arrow_right_above_arrow_left.svg" width="15px"> Add **pickup\_truck\_and\_arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_under_taxi_checkerboard.svg" width="15px"> Add **pickup\_truck\_under\_taxi\_checkerboard** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_and_locked_lock_with_keyhole.svg" width="15px"> Add **pickup\_truck\_and\_locked\_lock\_with\_keyhole** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickup_truck_under_list_beside_checkmark.svg" width="15px"> Add **pickup\_truck\_under\_list\_beside\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_people_above_pickup_truck.svg" width="15px"> Add **two\_people\_above\_pickup\_truck** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/taxi_under_key.svg" width="15px"> Add **taxi\_under\_key** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/taxi_under_wrench.svg" width="15px"> Add **taxi\_under\_wrench** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/keyboard.svg" width="15px"> Add **keyboard** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/keyboard_in_rectangle.svg" width="15px"> Add **keyboard\_in\_rectangle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/one_pip.svg" width="15px"> Add **one\_pip** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_pips.svg" width="15px"> Add **two\_pips** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_pips.svg" width="15px"> Add **three\_pips** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/four_pips.svg" width="15px"> Add **four\_pips** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/five_pips.svg" width="15px"> Add **five\_pips** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/six_pips.svg" width="15px"> Add **six\_pips** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/bowling_pin.svg" width="15px"> Add **bowling\_pin** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/candlepin.svg" width="15px"> Add **candlepin** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/deer_with_antlers_under_checkmark.svg" width="15px"> Add **deer\_with\_antlers\_under\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/deer_head_under_paragraph.svg" width="15px"> Add **deer\_head\_under\_paragraph** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/deer_head_under_list_beside_checkmark.svg" width="15px"> Add **deer\_head\_under\_list\_beside\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/deer_head_with_antlers_on_shield_mount.svg" width="15px"> Add **deer\_head\_with\_antlers\_on\_shield\_mount** by [@quincylvania](https://github.com/quincylvania) ([#250](https://github.com/waysidemapping/pinhead/issues/250))
* <img src="https://pinhead.ink/v26/badge_shield_with_deer_head_with_antlers.svg" width="15px"> Add **badge\_shield\_with\_deer\_head\_with\_antlers** by [@quincylvania](https://github.com/quincylvania) ([#250](https://github.com/waysidemapping/pinhead/issues/250))
* <img src="https://pinhead.ink/v26/egg_with_crack.svg" width="15px"> Add **egg\_with\_crack** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/badminton_racket.svg" width="15px"> Add **badminton\_racket** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pickleball_paddle.svg" width="15px"> Add **pickleball\_paddle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/table_tennis_paddle_and_ball.svg" width="15px"> Add **table\_tennis\_paddle\_and\_ball** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/groin_with_rememberance_ribbon.svg" width="15px"> Add **groin\_with\_rememberance\_ribbon** from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
* <img src="https://pinhead.ink/v26/groin.svg" width="15px"> Add **groin** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/list_beside_checkmark.svg" width="15px"> Add **list\_beside\_checkmark** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cc_uppercase_above_caption.svg" width="15px"> Add **cc\_uppercase\_above\_caption** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/tv_screen.svg" width="15px"> Add **tv\_screen** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cc_uppercase_in_tv_screen.svg" width="15px"> Add **cc\_uppercase\_in\_tv\_screen** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/oc_uppercase_above_caption.svg" width="15px"> Add **oc\_uppercase\_above\_caption** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/oc_uppercase_in_tv_screen.svg" width="15px"> Add **oc\_uppercase\_in\_tv\_screen** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/sitting_tank_toilet_and_wc_uppercase.svg" width="15px"> Add **sitting\_tank\_toilet\_and\_wc\_uppercase** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/111.svg" width="15px"> Add **111** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/112.svg" width="15px"> Add **112** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/123.svg" width="15px"> Add **123** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/211.svg" width="15px"> Add **211** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/311.svg" width="15px"> Add **311** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/411.svg" width="15px"> Add **411** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/511.svg" width="15px"> Add **511** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/611.svg" width="15px"> Add **611** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/711.svg" width="15px"> Add **711** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/811.svg" width="15px"> Add **811** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/988.svg" width="15px"> Add **988** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/999.svg" width="15px"> Add **999** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_chevrons_right.svg" width="15px"> Add **three\_chevrons\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_right_above_arrow_left.svg" width="15px"> Add **arrow\_right\_above\_arrow\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_up_beside_arrow_down.svg" width="15px"> Add **arrow\_up\_beside\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrows_up_down.svg" width="15px"> Add **arrows\_up\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrows_top_left_bottom_right.svg" width="15px"> Add **arrows\_top\_left\_bottom\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrows_bottom_left_top_right.svg" width="15px"> Add **arrows\_bottom\_left\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_bottom_right_beside_arrow_bottom_left_above_arrow_top_right_beside_arrow_top_left.svg" width="15px"> Add **arrow\_bottom\_right\_beside\_arrow\_bottom\_left\_above\_arrow\_top\_right\_beside\_arrow\_top\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_down_above_arrow_right_beside_arrow_left_above_arrow_up.svg" width="15px"> Add **arrow\_down\_above\_arrow\_right\_beside\_arrow\_left\_above\_arrow\_up** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_top_left_beside_arrow_top_right_above_arrow_bottom_left_beside_arrow_bottom_right.svg" width="15px"> Add **arrow\_top\_left\_beside\_arrow\_top\_right\_above\_arrow\_bottom\_left\_beside\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrows_top_left_bottom_right_bottom_left_top_right.svg" width="15px"> Add **arrows\_top\_left\_bottom\_right\_bottom\_left\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_up_above_arrow_left_beside_arrow_right_above_arrow_down.svg" width="15px"> Add **arrow\_up\_above\_arrow\_left\_beside\_arrow\_right\_above\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrows_up_down_left_right.svg" width="15px"> Add **arrows\_up\_down\_left\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/wide_p_and_arrow_down.svg" width="15px"> Add **wide\_p\_and\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/wide_e_and_arrow_down.svg" width="15px"> Add **wide\_e\_and\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/circle_with_vertical_bar.svg" width="15px"> Add **circle\_with\_vertical\_bar** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_up.svg" width="15px"> Add **triangle\_up** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangle_up_with_plus.svg" width="15px"> Add **triangle\_up\_with\_plus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_down.svg" width="15px"> Add **triangle\_down** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangle_down_with_plus.svg" width="15px"> Add **triangle\_down\_with\_plus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_left.svg" width="15px"> Add **triangle\_left** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangle_left_with_plus.svg" width="15px"> Add **triangle\_left\_with\_plus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_right.svg" width="15px"> Add **triangle\_right** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/triangle_right_with_plus.svg" width="15px"> Add **triangle\_right\_with\_plus** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_up_outline.svg" width="15px"> Add **triangle\_up\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_down_outline.svg" width="15px"> Add **triangle\_down\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_left_outline.svg" width="15px"> Add **triangle\_left\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/triangle_right_outline.svg" width="15px"> Add **triangle\_right\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_triangle_up_with_question_mark.svg" width="15px"> Add **rounded\_triangle\_up\_with\_question\_mark** by [@quincylvania](https://github.com/quincylvania) ([#383](https://github.com/waysidemapping/pinhead/issues/383))
* <img src="https://pinhead.ink/v26/rounded_triangle_left.svg" width="15px"> Add **rounded\_triangle\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_triangle_right.svg" width="15px"> Add **rounded\_triangle\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_triangle_left_outline.svg" width="15px"> Add **rounded\_triangle\_left\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_triangle_right_outline.svg" width="15px"> Add **rounded\_triangle\_right\_outline** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/square.svg" width="15px"> Add **square** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/square_with_dot.svg" width="15px"> Add **square\_with\_dot** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/square_with_square_dot.svg" width="15px"> Add **square\_with\_square\_dot** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/square_outline.svg" width="15px"> Add **square\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/square_outline_with_bottom_right_half.svg" width="15px"> Add **square\_outline\_with\_bottom\_right\_half** by [@quincylvania](https://github.com/quincylvania) ([#462](https://github.com/waysidemapping/pinhead/issues/462))
* <img src="https://pinhead.ink/v26/square_outline_with_top_left_half.svg" width="15px"> Add **square\_outline\_with\_top\_left\_half** by [@quincylvania](https://github.com/quincylvania) ([#462](https://github.com/waysidemapping/pinhead/issues/462))
* <img src="https://pinhead.ink/v26/square_outline_with_dot.svg" width="15px"> Add **square\_outline\_with\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/square_outline_with_square_dot.svg" width="15px"> Add **square\_outline\_with\_square\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_square_outline_with_dot.svg" width="15px"> Add **rounded\_square\_outline\_with\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/rounded_square_outline_with_square_dot.svg" width="15px"> Add **rounded\_square\_outline\_with\_square\_dot** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/arrow_top_right_from_square_outline.svg" width="15px"> Add **arrow\_top\_right\_from\_square\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/horizontal_bar.svg" width="15px"> Add **horizontal\_bar** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/vertical_bar.svg" width="15px"> Add **vertical\_bar** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/wide_rectangle.svg" width="15px"> Add **wide\_rectangle** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/wide_rectangle_outline.svg" width="15px"> Add **wide\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/tall_rectangle.svg" width="15px"> Add **tall\_rectangle** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/tall_rectangle_outline.svg" width="15px"> Add **tall\_rectangle\_outline** by [@quincylvania](https://github.com/quincylvania) ([#451](https://github.com/waysidemapping/pinhead/issues/451))
* <img src="https://pinhead.ink/v26/two_tall_rectangles_top_left.svg" width="15px"> Add **two\_tall\_rectangles\_top\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/two_tall_rectangles_top_right.svg" width="15px"> Add **two\_tall\_rectangles\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_tall_rectangles_left.svg" width="15px"> Add **three\_tall\_rectangles\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_tall_rectangles_right.svg" width="15px"> Add **three\_tall\_rectangles\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_tall_rectangles_up.svg" width="15px"> Add **three\_tall\_rectangles\_up** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/three_tall_rectangles_down.svg" width="15px"> Add **three\_tall\_rectangles\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_tall_rectangle.svg" width="15px"> Add **cairn\_and\_tall\_rectangle** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_two_tall_rectangles_top_left.svg" width="15px"> Add **cairn\_and\_two\_tall\_rectangles\_top\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_two_tall_rectangles_top_right.svg" width="15px"> Add **cairn\_and\_two\_tall\_rectangles\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_three_tall_rectangles_left.svg" width="15px"> Add **cairn\_and\_three\_tall\_rectangles\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_three_tall_rectangles_right.svg" width="15px"> Add **cairn\_and\_three\_tall\_rectangles\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_three_tall_rectangles_up.svg" width="15px"> Add **cairn\_and\_three\_tall\_rectangles\_up** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cairn_and_three_tall_rectangles_down.svg" width="15px"> Add **cairn\_and\_three\_tall\_rectangles\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cartoon_cannon.svg" width="15px"> Add **cartoon\_cannon** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/cartoon_bomb.svg" width="15px"> Add **cartoon\_bomb** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_international_wheelchair_symbol.svg" width="15px"> Add **pixel\_international\_wheelchair\_symbol** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_palm_tree.svg" width="15px"> Add **pixel\_palm\_tree** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_canoe.svg" width="15px"> Add **pixel\_canoe** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_canoe_above_water.svg" width="15px"> Add **pixel\_canoe\_above\_water** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrows_left_right.svg" width="15px"> Add **pixel\_arrows\_left\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrows_up_down.svg" width="15px"> Add **pixel\_arrows\_up\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_up.svg" width="15px"> Add **pixel\_arrow\_up** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_down.svg" width="15px"> Add **pixel\_arrow\_down** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_left.svg" width="15px"> Add **pixel\_arrow\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_right.svg" width="15px"> Add **pixel\_arrow\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_top_right.svg" width="15px"> Add **pixel\_arrow\_top\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_bottom_right.svg" width="15px"> Add **pixel\_arrow\_bottom\_right** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_bottom_left.svg" width="15px"> Add **pixel\_arrow\_bottom\_left** by [@quincylvania](https://github.com/quincylvania)
* <img src="https://pinhead.ink/v26/pixel_arrow_top_left.svg" width="15px"> Add **pixel\_arrow\_top\_left** by [@quincylvania](https://github.com/quincylvania)

## [15.25.0] - 2026-07-04

_Pinhead v25_

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v24/fillet_knife_and_fish.svg" width="15px"/> `fillet_knife_and_fish` -> <img src="https://pinhead.ink/v25/fish_under_fillet_knife.svg" width="15px"/> `fish_under_fillet_knife` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/fish_and_hook.svg" width="15px"/> `fish_and_hook` -> <img src="https://pinhead.ink/v25/fish_under_barbed_hook.svg" width="15px"/> `fish_under_barbed_hook` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/fish_and_hook_under_ice.svg" width="15px"/> `fish_and_hook_under_ice` -> <img src="https://pinhead.ink/v25/fish_head_beside_barbed_hook_on_line_under_ice.svg" width="15px"/> `fish_head_beside_barbed_hook_on_line_under_ice` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/inscribed_stone.svg" width="15px"/> `inscribed_stone` -> <img src="https://pinhead.ink/v25/round_rock_with_inscription.svg" width="15px"/> `round_rock_with_inscription` by [@quincylvania](https://github.com/quincylvania)

### Renamed icons

- <img src="https://pinhead.ink/v25/open_scissors.svg" width="15px"/> `scissors_open` -> `open_scissors`

### Redesigned icons

- <img src="https://pinhead.ink/v24/car_in_gable_roofed_building.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/car_in_gable_roofed_building.svg" width="15px"/> `car_in_gable_roofed_building` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/fillet_knife.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/fillet_knife.svg" width="15px"/> `fillet_knife` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/fish.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/fish.svg" width="15px"/> `fish` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/fishes.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/fishes.svg" width="15px"/> `fishes` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/memorial_stone.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/memorial_stone.svg" width="15px"/> `memorial_stone` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/memorial_stone_with_inscription.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/memorial_stone_with_inscription.svg" width="15px"/> `memorial_stone_with_inscription` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/key.svg" width="15px"/> `key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorboat_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorboat_and_key.svg" width="15px"/> `motorboat_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorboat_and_wrench.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorboat_and_wrench.svg" width="15px"/> `motorboat_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/spiky_fish.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/spiky_fish.svg" width="15px"/> `spiky_fish` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/spiky_fish_with_x.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/spiky_fish_with_x.svg" width="15px"/> `spiky_fish_with_x` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/bear_spray_can_with_spray.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/bear_spray_can_with_spray.svg" width="15px"/> `bear_spray_can_with_spray` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/car_and_wrench.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/car_and_wrench.svg" width="15px"/> `car_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/bicycle_and_wrench.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/bicycle_and_wrench.svg" width="15px"/> `bicycle_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorcycle_and_wrench.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorcycle_and_wrench.svg" width="15px"/> `motorcycle_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorboat_and_wrench.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorboat_and_wrench.svg" width="15px"/> `motorboat_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/car_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/car_and_key.svg" width="15px"/> `car_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/bicycle_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/bicycle_and_key.svg" width="15px"/> `bicycle_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorcycle_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorcycle_and_key.svg" width="15px"/> `motorcycle_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/motorboat_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/motorboat_and_key.svg" width="15px"/> `motorboat_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/suitcase_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/suitcase_and_key.svg" width="15px"/> `suitcase_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/garage_and_key.svg" width="15px"/> -> <img src="https://pinhead.ink/v25/garage_and_key.svg" width="15px"/> `garage_and_key` by [@quincylvania](https://github.com/quincylvania)

### Added icons

- <img src="https://pinhead.ink/v25/canoe.svg" width="15px"/> Add `canoe` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_on_water.svg" width="15px"/> Add `canoe_on_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/button.svg" width="15px"/> Add `button` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/paintbrush.svg" width="15px"/> Add `paintbrush` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/hammer_and_nail.svg" width="15px"/> Add `hammer_and_nail` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/tabletop_microphone.svg" width="15px"/> Add `tabletop_microphone` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/bell.svg" width="15px"/> Add `bell` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/classical_statue.svg" width="15px"/> Add `classical_statue` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/bucket.svg" width="15px"/> Add `bucket` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/clapperboard.svg" width="15px"/> Add `clapperboard` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/coffin_with_latin_cross.svg" width="15px"/> Add `coffin_with_latin_cross` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/coffin.svg" width="15px"/> Add `coffin` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/telegraph_key.svg" width="15px"/> Add `telegraph_key` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/horizontal_storage_tank_on_supports.svg" width="15px"/> Add `horizontal_storage_tank_on_supports` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/lantern_lamppost.svg" width="15px"/> Add `lantern_lamppost` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/tshirt_on_clothes_hanger_and_folded_linens.svg" width="15px"/> Add `tshirt_on_clothes_hanger_and_folded_linens` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/person_running_after_person.svg" width="15px"/> Add `person_running_after_person` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/car_wheel_with_tire.svg" width="15px"/> Add `car_wheel_with_tire` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/screw_beside_nail.svg" width="15px"/> Add `screw_beside_nail` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/open_scissors_crossing_handled_comb.svg" width="15px"/> Add `open_scissors_crossing_handled_comb` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/open_book_under_roof.svg" width="15px"/> Add `open_book_under_roof` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v25/gable_roofed_building.svg" width="15px"/> Add `gable_roofed_building` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tabletop_microphone_in_gable_roofed_building.svg" width="15px"/> Add `tabletop_microphone_in_gable_roofed_building` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/cc_text.svg" width="15px"/> Add `cc_text` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/oc_text.svg" width="15px"/> Add `oc_text` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/art_text.svg" width="15px"/> Add `art_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/art_text_above_swash_line.svg" width="15px"/> Add `art_text_above_swash_line` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/ear_atop_slash_with_t.svg" width="15px"/> Add `ear_atop_slash_with_t` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/traffic_cone_and_exclamation_point.svg" width="15px"/> Add `traffic_cone_and_exclamation_point` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v25/hook.svg" width="15px"/> Add `hook` by [@quincylvania](https://github.com/quincylvania) ([#195](https://github.com/waysidemapping/pinhead/issues/195))
- <img src="https://pinhead.ink/v25/barbed_hook.svg" width="15px"/> Add `barbed_hook` by [@quincylvania](https://github.com/quincylvania) ([#195](https://github.com/waysidemapping/pinhead/issues/195))
- <img src="https://pinhead.ink/v25/fish_under_water.svg" width="15px"/> Add `fish_under_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/spiky_fish_under_water.svg" width="15px"/> Add `spiky_fish_under_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/angelfish_under_water.svg" width="15px"/> Add `angelfish_under_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/fish_head.svg" width="15px"/> Add `fish_head` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/fish_head_beside_barbed_hook_on_line.svg" width="15px"/> Add `fish_head_beside_barbed_hook_on_line` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/fish_head_beside_barbed_hook_on_line_under_water.svg" width="15px"/> Add `fish_head_beside_barbed_hook_on_line_under_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/fish_head_beside_barbed_hook_under_paragraph.svg" width="15px"/> Add `fish_head_beside_barbed_hook_under_paragraph` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/round_rock.svg" width="15px"/> Add `round_rock` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/memorial_stone_with_latin_cross.svg" width="15px"/> Add `memorial_stone_with_latin_cross` by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/lowrise_apartment_building_on_ground.svg" width="15px"/> Add `lowrise_apartment_building_on_ground` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/officer.svg" width="15px"/> Add `officer` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/military_police_officer.svg" width="15px"/> Add `military_police_officer` by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/transit_vehicle_with_pantograph_on_railway_track.svg" width="15px"/> Add `transit_vehicle_with_pantograph_on_railway_track` by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/die_face_with_one_pip.svg" width="15px"/> Add `die_face_with_one_pip` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/die_face_with_two_pips.svg" width="15px"/> Add `die_face_with_two_pips` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/die_face_with_three_pips.svg" width="15px"/> Add `die_face_with_three_pips` by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/die_face_with_four_pips.svg" width="15px"/> Add `die_face_with_four_pips` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/die_face_with_five_pips.svg" width="15px"/> Add `die_face_with_five_pips` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/die_face_with_six_pips.svg" width="15px"/> Add `die_face_with_six_pips` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_dollar.svg" width="15px"/> Add `pin_pad_with_dollar` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/pin_pad_with_euro.svg" width="15px"/> Add `pin_pad_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_pound.svg" width="15px"/> Add `pin_pad_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_yen_yuan.svg" width="15px"/> Add `pin_pad_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_rupee.svg" width="15px"/> Add `pin_pad_with_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_ruble.svg" width="15px"/> Add `pin_pad_with_ruble` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_peso.svg" width="15px"/> Add `pin_pad_with_peso` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pin_pad_with_baht.svg" width="15px"/> Add `pin_pad_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/pin_pad_with_shekel.svg" width="15px"/> Add `pin_pad_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/open_envelope_right.svg" width="15px"/> Add `open_envelope_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_dollar.svg" width="15px"/> Add `open_envelope_right_with_dollar` from [OpenHistoricalMap](https://github.com/OpenHistoricalMap/map-styles) imported by [@quincylvania](https://github.com/quincylvania) ([#233](https://github.com/waysidemapping/pinhead/issues/233))
- <img src="https://pinhead.ink/v25/open_envelope_right_with_euro.svg" width="15px"/> Add `open_envelope_right_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_pound.svg" width="15px"/> Add `open_envelope_right_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_yen_yuan.svg" width="15px"/> Add `open_envelope_right_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_rupee.svg" width="15px"/> Add `open_envelope_right_with_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_ruble.svg" width="15px"/> Add `open_envelope_right_with_ruble` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_peso.svg" width="15px"/> Add `open_envelope_right_with_peso` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/open_envelope_right_with_baht.svg" width="15px"/> Add `open_envelope_right_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/open_envelope_right_with_shekel.svg" width="15px"/> Add `open_envelope_right_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/key_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `key_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/suitcase_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `suitcase_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/car_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `car_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/taxi_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `taxi_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bicycle_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `bicycle_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/cargobike_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `cargobike_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `motorcycle_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `motorboat_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `canoe_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/garage_and_wrench.svg" width="15px"/> Add `garage_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/campsite_under_paragraph.svg" width="15px"/> Add `campsite_under_paragraph` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/spiky_fish_under_paragraph.svg" width="15px"/> Add `spiky_fish_under_paragraph` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/fish_under_paragraph.svg" width="15px"/> Add `fish_under_paragraph` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/person_driving_motorboat_on_water_under_paragraph.svg" width="15px"/> Add `person_driving_motorboat_on_water_under_paragraph` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/car_under_list_beside_checkmark.svg" width="15px"/> Add `car_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v25/bicycle_under_list_beside_checkmark.svg" width="15px"/> Add `bicycle_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/cargobike_under_list_beside_checkmark.svg" width="15px"/> Add `cargobike_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_under_list_beside_checkmark.svg" width="15px"/> Add `motorcycle_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_under_list_beside_checkmark.svg" width="15px"/> Add `motorboat_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_under_list_beside_checkmark.svg" width="15px"/> Add `canoe_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/suitcase_under_list_beside_checkmark.svg" width="15px"/> Add `suitcase_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/campsite_under_list_beside_checkmark.svg" width="15px"/> Add `campsite_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/fish_under_list_beside_checkmark.svg" width="15px"/> Add `fish_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/spiky_fish_under_list_beside_checkmark.svg" width="15px"/> Add `spiky_fish_under_list_beside_checkmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/people_above_car.svg" width="15px"/> Add `people_above_car` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v25/bear_spray_can.svg" width="15px"/> Add `bear_spray_can` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_arrow_right_above_arrow_left.svg" width="15px"/> Add `bear_spray_can_with_spray_and_arrow_right_above_arrow_left` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_recycling_symbol.svg" width="15px"/> Add `bear_spray_can_with_spray_and_recycling_symbol` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_dollar.svg" width="15px"/> Add `bear_spray_can_with_spray_and_dollar` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_euro.svg" width="15px"/> Add `bear_spray_can_with_spray_and_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_pound.svg" width="15px"/> Add `bear_spray_can_with_spray_and_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_yen_yuan.svg" width="15px"/> Add `bear_spray_can_with_spray_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_rupee.svg" width="15px"/> Add `bear_spray_can_with_spray_and_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_ruble.svg" width="15px"/> Add `bear_spray_can_with_spray_and_ruble` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_peso.svg" width="15px"/> Add `bear_spray_can_with_spray_and_peso` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_shekel.svg" width="15px"/> Add `bear_spray_can_with_spray_and_shekel` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bear_spray_can_with_spray_and_baht.svg" width="15px"/> Add `bear_spray_can_with_spray_and_baht` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/taxi_checkerboard.svg" width="15px"/> Add `taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/taxi_and_taxi_checkerboard.svg" width="15px"/> Add `taxi_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bicycle_and_taxi_checkerboard.svg" width="15px"/> Add `bicycle_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/cargobike_and_taxi_checkerboard.svg" width="15px"/> Add `cargobike_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_taxi_checkerboard.svg" width="15px"/> Add `motorcycle_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_taxi_checkerboard.svg" width="15px"/> Add `motorboat_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_and_taxi_checkerboard.svg" width="15px"/> Add `canoe_and_taxi_checkerboard` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/car_and_locked_lock_with_keyhole.svg" width="15px"/> Add `car_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/bicycle_and_locked_lock_with_keyhole.svg" width="15px"/> Add `bicycle_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/cargobike_and_locked_lock_with_keyhole.svg" width="15px"/> Add `cargobike_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_locked_lock_with_keyhole.svg" width="15px"/> Add `motorcycle_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_locked_lock_with_keyhole.svg" width="15px"/> Add `motorboat_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_and_locked_lock_with_keyhole.svg" width="15px"/> Add `canoe_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/suitcase_and_locked_lock_with_keyhole.svg" width="15px"/> Add `suitcase_and_locked_lock_with_keyhole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_and_key.svg" width="15px"/> Add `canoe_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/canoe_and_tag.svg" width="15px"/> Add `canoe_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/cargobike_and_wrench.svg" width="15px"/> Add `cargobike_and_wrench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/cargobike_and_key.svg" width="15px"/> Add `cargobike_and_key` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/suitcase_in_rectangle_outline_and_key.svg" width="15px"/> Add `suitcase_in_rectangle_outline_and_key` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v25/motorcycle_and_dollar.svg" width="15px"/> Add `motorcycle_and_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_euro.svg" width="15px"/> Add `motorcycle_and_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_pound.svg" width="15px"/> Add `motorcycle_and_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_yen_yuan.svg" width="15px"/> Add `motorcycle_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_rupee.svg" width="15px"/> Add `motorcycle_and_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_ruble.svg" width="15px"/> Add `motorcycle_and_ruble` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_peso.svg" width="15px"/> Add `motorcycle_and_peso` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_baht.svg" width="15px"/> Add `motorcycle_and_baht` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorcycle_and_shekel.svg" width="15px"/> Add `motorcycle_and_shekel` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_dollar.svg" width="15px"/> Add `motorboat_and_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_euro.svg" width="15px"/> Add `motorboat_and_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_pound.svg" width="15px"/> Add `motorboat_and_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_yen_yuan.svg" width="15px"/> Add `motorboat_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_rupee.svg" width="15px"/> Add `motorboat_and_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_ruble.svg" width="15px"/> Add `motorboat_and_ruble` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_peso.svg" width="15px"/> Add `motorboat_and_peso` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_baht.svg" width="15px"/> Add `motorboat_and_baht` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/motorboat_and_shekel.svg" width="15px"/> Add `motorboat_and_shekel` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/shekel.svg" width="15px"/> Add `shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/person_using_terminal_kiosk_with_shekel.svg" width="15px"/> Add `person_using_terminal_kiosk_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/shopping_bag_with_shekel.svg" width="15px"/> Add `shopping_bag_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/milk_carton_and_apple_and_shekel.svg" width="15px"/> Add `milk_carton_and_apple_and_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/car_with_shekel.svg" width="15px"/> Add `car_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/bicycle_and_shekel.svg" width="15px"/> Add `bicycle_and_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/cargobike_and_shekel.svg" width="15px"/> Add `cargobike_and_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/campsite_with_shekel.svg" width="15px"/> Add `campsite_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/tipi_campsite_with_shekel.svg" width="15px"/> Add `tipi_campsite_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/tag_with_shekel.svg" width="15px"/> Add `tag_with_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/baht.svg" width="15px"/> Add `baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/person_using_terminal_kiosk_with_baht.svg" width="15px"/> Add `person_using_terminal_kiosk_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/shopping_bag_with_baht.svg" width="15px"/> Add `shopping_bag_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/milk_carton_and_apple_and_baht.svg" width="15px"/> Add `milk_carton_and_apple_and_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/car_with_baht.svg" width="15px"/> Add `car_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/bicycle_and_baht.svg" width="15px"/> Add `bicycle_and_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/cargobike_and_baht.svg" width="15px"/> Add `cargobike_and_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/campsite_with_baht.svg" width="15px"/> Add `campsite_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/tipi_campsite_with_baht.svg" width="15px"/> Add `tipi_campsite_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/tag_with_baht.svg" width="15px"/> Add `tag_with_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/angry_face.svg" width="15px"/> Add `angry_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/anguished_face.svg" width="15px"/> Add `anguished_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/anguished_face_with_spots.svg" width="15px"/> Add `anguished_face_with_spots` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/calm_face.svg" width="15px"/> Add `calm_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/confused_face.svg" width="15px"/> Add `confused_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face.svg" width="15px"/> Add `coughing_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_with_spittle.svg" width="15px"/> Add `coughing_face_with_spittle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_with_phlegm.svg" width="15px"/> Add `coughing_face_with_phlegm` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/face_with_tongue_out.svg" width="15px"/> Add `face_with_tongue_out` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/vomiting_face.svg" width="15px"/> Add `vomiting_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/frowning_face_with_head_bandage.svg" width="15px"/> Add `frowning_face_with_head_bandage` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/laughing_face.svg" width="15px"/> Add `laughing_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/nauseous_face.svg" width="15px"/> Add `nauseous_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/nervous_face.svg" width="15px"/> Add `nervous_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/neutral_face.svg" width="15px"/> Add `neutral_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sad_face.svg" width="15px"/> Add `sad_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sad_face_with_tear.svg" width="15px"/> Add `sad_face_with_tear` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/happy_face.svg" width="15px"/> Add `happy_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/happy_face_with_face_mask.svg" width="15px"/> Add `happy_face_with_face_mask` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/smiling_face.svg" width="15px"/> Add `smiling_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/smiling_face_with_eyeglasses.svg" width="15px"/> Add `smiling_face_with_eyeglasses` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sobbing_face.svg" width="15px"/> Add `sobbing_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/surprised_face.svg" width="15px"/> Add `surprised_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/surprised_face_with_x_eyes.svg" width="15px"/> Add `surprised_face_with_x_eyes` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face.svg" width="15px"/> Add `tired_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_sweat.svg" width="15px"/> Add `tired_face_with_sweat` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_oral_thermometer_and_brow_sweat.svg" width="15px"/> Add `tired_face_with_oral_thermometer_and_brow_sweat` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_z.svg" width="15px"/> Add `tired_face_with_z` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/woozy_face.svg" width="15px"/> Add `woozy_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/angry_face_in_circle_outline.svg" width="15px"/> Add `angry_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/anguished_face_in_circle_outline.svg" width="15px"/> Add `anguished_face_in_circle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/anguished_face_with_spots_in_circle_outline.svg" width="15px"/> Add `anguished_face_with_spots_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/calm_face_in_circle_outline.svg" width="15px"/> Add `calm_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/confused_face_in_circle_outline.svg" width="15px"/> Add `confused_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/coughing_face_in_circle_outline.svg" width="15px"/> Add `coughing_face_in_circle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_with_spittle_in_circle_outline.svg" width="15px"/> Add `coughing_face_with_spittle_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/coughing_face_with_phlegm_in_circle_outline.svg" width="15px"/> Add `coughing_face_with_phlegm_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/face_with_tongue_out_in_circle_outline.svg" width="15px"/> Add `face_with_tongue_out_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/vomiting_face_in_circle_outline.svg" width="15px"/> Add `vomiting_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/frowning_face_with_head_bandage_in_circle_outline.svg" width="15px"/> Add `frowning_face_with_head_bandage_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/laughing_face_in_circle_outline.svg" width="15px"/> Add `laughing_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/nauseous_face_in_circle_outline.svg" width="15px"/> Add `nauseous_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/nervous_face_in_circle_outline.svg" width="15px"/> Add `nervous_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/neutral_face_in_circle_outline.svg" width="15px"/> Add `neutral_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/sad_face_in_circle_outline.svg" width="15px"/> Add `sad_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/sad_face_with_tear_in_circle_outline.svg" width="15px"/> Add `sad_face_with_tear_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/happy_face_in_circle_outline.svg" width="15px"/> Add `happy_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/happy_face_with_face_mask_in_circle_outline.svg" width="15px"/> Add `happy_face_with_face_mask_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/smiling_face_in_circle_outline.svg" width="15px"/> Add `smiling_face_in_circle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/smiling_face_with_eyeglasses_in_circle_outline.svg" width="15px"/> Add `smiling_face_with_eyeglasses_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/sobbing_face_in_circle_outline.svg" width="15px"/> Add `sobbing_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/surprised_face_in_circle_outline.svg" width="15px"/> Add `surprised_face_in_circle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/surprised_face_with_x_eyes_in_circle_outline.svg" width="15px"/> Add `surprised_face_with_x_eyes_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/tired_face_in_circle_outline.svg" width="15px"/> Add `tired_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/tired_face_with_sweat_in_circle_outline.svg" width="15px"/> Add `tired_face_with_sweat_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/tired_face_with_oral_thermometer_and_brow_sweat_in_circle_outline.svg" width="15px"/> Add `tired_face_with_oral_thermometer_and_brow_sweat_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/tired_face_with_z_in_circle_outline.svg" width="15px"/> Add `tired_face_with_z_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/woozy_face_in_circle_outline.svg" width="15px"/> Add `woozy_face_in_circle_outline` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v25/angry_face_in_circle.svg" width="15px"/> Add `angry_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/anguished_face_in_circle.svg" width="15px"/> Add `anguished_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/anguished_face_with_spots_in_circle.svg" width="15px"/> Add `anguished_face_with_spots_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/calm_face_in_circle.svg" width="15px"/> Add `calm_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/confused_face_in_circle.svg" width="15px"/> Add `confused_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_in_circle.svg" width="15px"/> Add `coughing_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_with_spittle_in_circle.svg" width="15px"/> Add `coughing_face_with_spittle_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/coughing_face_with_phlegm_in_circle.svg" width="15px"/> Add `coughing_face_with_phlegm_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/face_with_tongue_out_in_circle.svg" width="15px"/> Add `face_with_tongue_out_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/vomiting_face_in_circle.svg" width="15px"/> Add `vomiting_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/frowning_face_with_head_bandage_in_circle.svg" width="15px"/> Add `frowning_face_with_head_bandage_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/laughing_face_in_circle.svg" width="15px"/> Add `laughing_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/nauseous_face_in_circle.svg" width="15px"/> Add `nauseous_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/nervous_face_in_circle.svg" width="15px"/> Add `nervous_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/neutral_face_in_circle.svg" width="15px"/> Add `neutral_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sad_face_in_circle.svg" width="15px"/> Add `sad_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sad_face_with_tear_in_circle.svg" width="15px"/> Add `sad_face_with_tear_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/happy_face_in_circle.svg" width="15px"/> Add `happy_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/happy_face_with_face_mask_in_circle.svg" width="15px"/> Add `happy_face_with_face_mask_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/smiling_face_in_circle.svg" width="15px"/> Add `smiling_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/smiling_face_with_eyeglasses_in_circle.svg" width="15px"/> Add `smiling_face_with_eyeglasses_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/sobbing_face_in_circle.svg" width="15px"/> Add `sobbing_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/surprised_face_in_circle.svg" width="15px"/> Add `surprised_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/surprised_face_with_x_eyes_in_circle.svg" width="15px"/> Add `surprised_face_with_x_eyes_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_in_circle.svg" width="15px"/> Add `tired_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_sweat_in_circle.svg" width="15px"/> Add `tired_face_with_sweat_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_oral_thermometer_and_brow_sweat_in_circle.svg" width="15px"/> Add `tired_face_with_oral_thermometer_and_brow_sweat_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/tired_face_with_z_in_circle.svg" width="15px"/> Add `tired_face_with_z_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/woozy_face_in_circle.svg" width="15px"/> Add `woozy_face_in_circle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pixel_shekel.svg" width="15px"/> Add `pixel_shekel` by [@quincylvania](https://github.com/quincylvania) ([#154](https://github.com/waysidemapping/pinhead/issues/154))
- <img src="https://pinhead.ink/v25/pixel_baht.svg" width="15px"/> Add `pixel_baht` by [@quincylvania](https://github.com/quincylvania) ([#243](https://github.com/waysidemapping/pinhead/issues/243))
- <img src="https://pinhead.ink/v25/pixel_bell.svg" width="15px"/> Add `pixel_bell` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pixel_fork_and_knife.svg" width="15px"/> Add `pixel_fork_and_knife` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pixel_water.svg" width="15px"/> Add `pixel_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pixel_waters.svg" width="15px"/> Add `pixel_waters` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v25/pixel_arrows_left_right_above_water.svg" width="15px"/> Add `pixel_arrows_left_right_above_water` by [@quincylvania](https://github.com/quincylvania)

## [15.24.0] - 2026-05-27

_Pinhead v24_

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v23/roof_with_fireplace_and_chimney.svg" width="15px"/> `roof_with_fireplace_and_chimney` -> <img src="https://pinhead.ink/v24/gable_roofed_shelter_with_fireplace_and_chimney.svg" width="15px"/> `gable_roofed_shelter_with_fireplace_and_chimney` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_building.svg" width="15px"/> `person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_building` -> <img src="https://pinhead.ink/v24/person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_shelter.svg" width="15px"/> `person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_shelter` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/snowflake_and_icicles.svg" width="15px"/> `snowflake_and_icicles` -> <img src="https://pinhead.ink/v24/snowflake_above_icicles.svg" width="15px"/> `snowflake_above_icicles` by [@quincylvania](https://github.com/quincylvania)

### Renamed icons

- <img src="https://pinhead.ink/v24/compass_rose_in_circle_outline.svg" width="15px"/> `compass_rose` -> `compass_rose_in_circle_outline`
- <img src="https://pinhead.ink/v24/rolled_curb.svg" width="15px"/> `kerb_rolled` -> `rolled_curb`
- <img src="https://pinhead.ink/v24/lowered_curb.svg" width="15px"/> `kerb_lowered` -> `lowered_curb`
- <img src="https://pinhead.ink/v24/flush_curb.svg" width="15px"/> `kerb_flush` -> `flush_curb`
- <img src="https://pinhead.ink/v24/raised_curb.svg" width="15px"/> `kerb_raised` -> `raised_curb`
- <img src="https://pinhead.ink/v24/rolled_curb_under_shoe.svg" width="15px"/> `kerb_rolled_under_shoe` -> `rolled_curb_under_shoe`
- <img src="https://pinhead.ink/v24/lowered_curb_under_shoe.svg" width="15px"/> `kerb_lowered_under_shoe` -> `lowered_curb_under_shoe`
- <img src="https://pinhead.ink/v24/flush_curb_under_shoe.svg" width="15px"/> `kerb_flush_under_shoe` -> `flush_curb_under_shoe`
- <img src="https://pinhead.ink/v24/raised_curb_under_shoe.svg" width="15px"/> `kerb_raised_under_shoe` -> `raised_curb_under_shoe`
- <img src="https://pinhead.ink/v24/car_beside_car_above_car_beside_car.svg" width="15px"/> `car_beside_car_under_car_beside_car` -> `car_beside_car_above_car_beside_car`
- <img src="https://pinhead.ink/v24/seaplane_takeoff_above_water.svg" width="15px"/> `seaplane_takeoff_over_water` -> `seaplane_takeoff_above_water`
- <img src="https://pinhead.ink/v24/flag_above_railway_track.svg" width="15px"/> `flag_over_railway_track` -> `flag_above_railway_track`

### Merged icons

- <img src="https://pinhead.ink/v23/zero_with_slash.svg" width="15px"/> `zero_with_slash` -> <img src="https://pinhead.ink/v24/zero.svg" width="15px"/> `zero`

### Redesigned icons

- <img src="https://pinhead.ink/v23/gasoline_pump.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/gasoline_pump.svg" width="15px"/> `gasoline_pump` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/person_slipping_down_cliff.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/person_slipping_down_cliff.svg" width="15px"/> `person_slipping_down_cliff` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/icicles.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/icicles.svg" width="15px"/> `icicles` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/exclamation_point.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/exclamation_point.svg" width="15px"/> `exclamation_point` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/zero.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/zero.svg" width="15px"/> `zero` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/map_pin_with_dot.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/map_pin_with_dot.svg" width="15px"/> `map_pin_with_dot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/map_pin.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/map_pin.svg" width="15px"/> `map_pin` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/map_pin_outline.svg" width="15px"/> -> <img src="https://pinhead.ink/v24/map_pin_outline.svg" width="15px"/> `map_pin_outline` by [@quincylvania](https://github.com/quincylvania)

### Added icons

- <img src="https://pinhead.ink/v24/person_holding_open_book_profile.svg" width="15px"/> Add `person_holding_open_book_profile` from [source](https://upload.wikimedia.org/wikipedia/commons/0/0f/MUTCD_I4-1.svg) imported by [@quincylvania](https://github.com/quincylvania) ([#41](https://github.com/waysidemapping/pinhead/issues/41))
- <img src="https://pinhead.ink/v24/person_sleeping_in_bed_above_car.svg" width="15px"/> Add `person_sleeping_in_bed_above_car` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40), [#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/person_sleeping_in_bed_between_floor_and_ceiling.svg" width="15px"/> Add `person_sleeping_in_bed_between_floor_and_ceiling` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/person_dropping_trash_into_wheelie_bin.svg" width="15px"/> Add `person_dropping_trash_into_wheelie_bin` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/column_shrine.svg" width="15px"/> Add `column_shrine` from [OSM Carto](https://github.com/openstreetmap-carto/openstreetmap-carto) imported by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/table_with_chairs.svg" width="15px"/> Add `table_with_chairs` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/table_with_umbrella_and_chairs.svg" width="15px"/> Add `table_with_umbrella_and_chairs` from [OSM Carto](https://github.com/openstreetmap-carto/openstreetmap-carto) imported by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/table_with_umbrella.svg" width="15px"/> Add `table_with_umbrella` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/compass_rose.svg" width="15px"/> Add `compass_rose` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/hot_dog.svg" width="15px"/> Add `hot_dog` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/martini_glass_and_wine_bottle.svg" width="15px"/> Add `martini_glass_and_wine_bottle` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/drink_can_and_drink_bottle.svg" width="15px"/> Add `drink_can_and_drink_bottle` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/beer_bottle_and_drink_bottle.svg" width="15px"/> Add `beer_bottle_and_drink_bottle` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/syrup_jug_and_droplet.svg" width="15px"/> Add `syrup_jug_and_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/gasoline_pump_with_d.svg" width="15px"/> Add `gasoline_pump_with_d` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/gasoline_pump_with_e.svg" width="15px"/> Add `gasoline_pump_with_e` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/globe_gasoline_pump.svg" width="15px"/> Add `globe_gasoline_pump` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/globe_gasoline_pump_with_d.svg" width="15px"/> Add `globe_gasoline_pump_with_d` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/globe_gasoline_pump_with_e.svg" width="15px"/> Add `globe_gasoline_pump_with_e` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/gable_roofed_shelter.svg" width="15px"/> Add `gable_roofed_shelter` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v24/gable_roofed_shelter_with_spoon_and_knife.svg" width="15px"/> Add `gable_roofed_shelter_with_spoon_and_knife` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v24/person_slipping_down_cliff_into_water.svg" width="15px"/> Add `person_slipping_down_cliff_into_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/person_sliding_down_cliff.svg" width="15px"/> Add `person_sliding_down_cliff` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/person_sliding_down_cliff_into_water.svg" width="15px"/> Add `person_sliding_down_cliff_into_water` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/ice_text.svg" width="15px"/> Add `ice_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/ice_text_above_icicles.svg" width="15px"/> Add `ice_text_above_icicles` by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v24/flush_curb_with_arrow_right.svg" width="15px"/> Add `flush_curb_with_arrow_right` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v24/lowered_curb_with_arrow_bottom_right.svg" width="15px"/> Add `lowered_curb_with_arrow_bottom_right` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v24/rolled_curb_with_arrow_bottom_right.svg" width="15px"/> Add `rolled_curb_with_arrow_bottom_right` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v24/raised_curb_with_arrow_down.svg" width="15px"/> Add `raised_curb_with_arrow_down` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v24/flush_curb_with_question_mark.svg" width="15px"/> Add `flush_curb_with_question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/lowered_curb_with_question_mark.svg" width="15px"/> Add `lowered_curb_with_question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/rolled_curb_with_question_mark.svg" width="15px"/> Add `rolled_curb_with_question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/raised_curb_with_question_mark.svg" width="15px"/> Add `raised_curb_with_question_mark` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v24/spherical_virus_with_exclamation_point.svg" width="15px"/> Add `spherical_virus_with_exclamation_point` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v24/question_mark.svg" width="15px"/> Add `question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/exclamation_point_beside_question_mark.svg" width="15px"/> Add `exclamation_point_beside_question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/exclamation_point_beside_exclamation_point.svg" width="15px"/> Add `exclamation_point_beside_exclamation_point` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/conifer_tree_beside_conifer_tree.svg" width="15px"/> Add `conifer_tree_beside_conifer_tree` by [@quincylvania](https://github.com/quincylvania) ([#228](https://github.com/waysidemapping/pinhead/issues/228))
- <img src="https://pinhead.ink/v24/campsite_beside_conifer_tree.svg" width="15px"/> Add `campsite_beside_conifer_tree` by [@quincylvania](https://github.com/quincylvania) ([#228](https://github.com/waysidemapping/pinhead/issues/228))
- <img src="https://pinhead.ink/v24/campsite_beside_conifer_tree_above_water.svg" width="15px"/> Add `campsite_beside_conifer_tree_above_water` by [@quincylvania](https://github.com/quincylvania) ([#228](https://github.com/waysidemapping/pinhead/issues/228))
- <img src="https://pinhead.ink/v24/oval_broadleaved_tree_beside_oval_broadleaved_tree.svg" width="15px"/> Add `oval_broadleaved_tree_beside_oval_broadleaved_tree` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/campsite_beside_oval_broadleaved_tree.svg" width="15px"/> Add `campsite_beside_oval_broadleaved_tree` by [@quincylvania](https://github.com/quincylvania) ([#228](https://github.com/waysidemapping/pinhead/issues/228))
- <img src="https://pinhead.ink/v24/campsite_beside_oval_broadleaved_tree_above_water.svg" width="15px"/> Add `campsite_beside_oval_broadleaved_tree_above_water` by [@quincylvania](https://github.com/quincylvania) ([#228](https://github.com/waysidemapping/pinhead/issues/228))
- <img src="https://pinhead.ink/v24/campsite_beside_campsite_above_campsite_beside_campsite.svg" width="15px"/> Add `campsite_beside_campsite_above_campsite_beside_campsite` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/campsite_on_platform.svg" width="15px"/> Add `campsite_on_platform` by [@quincylvania](https://github.com/quincylvania) ([#132](https://github.com/waysidemapping/pinhead/issues/132))
- <img src="https://pinhead.ink/v24/campsite_on_pier_in_water.svg" width="15px"/> Add `campsite_on_pier_in_water` by [@quincylvania](https://github.com/quincylvania) ([#133](https://github.com/waysidemapping/pinhead/issues/133))
- <img src="https://pinhead.ink/v24/campsite_above_water.svg" width="15px"/> Add `campsite_above_water` by [@quincylvania](https://github.com/quincylvania) ([#131](https://github.com/waysidemapping/pinhead/issues/131))
- <img src="https://pinhead.ink/v24/campsite_above_waters.svg" width="15px"/> Add `campsite_above_waters` by [@quincylvania](https://github.com/quincylvania) ([#131](https://github.com/waysidemapping/pinhead/issues/131))
- <img src="https://pinhead.ink/v24/arrows_left_right_above_waters.svg" width="15px"/> Add `arrows_left_right_above_waters` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v24/person_wearing_scuba_gear_diving_under_water.svg" width="15px"/> Add `person_wearing_scuba_gear_diving_under_water` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/exclamation_point_above_water.svg" width="15px"/> Add `exclamation_point_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/question_mark_above_water.svg" width="15px"/> Add `question_mark_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/zero_above_water.svg" width="15px"/> Add `zero_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/one_above_water.svg" width="15px"/> Add `one_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/one_minus_above_water.svg" width="15px"/> Add `one_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/one_plus_above_water.svg" width="15px"/> Add `one_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/one_minus.svg" width="15px"/> Add `one_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/one_plus.svg" width="15px"/> Add `one_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/two_above_water.svg" width="15px"/> Add `two_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/two_minus_above_water.svg" width="15px"/> Add `two_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/two_plus_above_water.svg" width="15px"/> Add `two_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/two_minus.svg" width="15px"/> Add `two_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/two_plus.svg" width="15px"/> Add `two_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/three_above_water.svg" width="15px"/> Add `three_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/three_minus_above_water.svg" width="15px"/> Add `three_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/three_plus_above_water.svg" width="15px"/> Add `three_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/three_minus.svg" width="15px"/> Add `three_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/three_plus.svg" width="15px"/> Add `three_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/four_above_water.svg" width="15px"/> Add `four_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/four_minus_above_water.svg" width="15px"/> Add `four_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/four_plus_above_water.svg" width="15px"/> Add `four_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/four_minus.svg" width="15px"/> Add `four_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/four_plus.svg" width="15px"/> Add `four_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/five_above_water.svg" width="15px"/> Add `five_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/five_minus_above_water.svg" width="15px"/> Add `five_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/five_plus_above_water.svg" width="15px"/> Add `five_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/five_minus.svg" width="15px"/> Add `five_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/five_plus.svg" width="15px"/> Add `five_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/six_above_water.svg" width="15px"/> Add `six_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/six_minus_above_water.svg" width="15px"/> Add `six_minus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/six_plus_above_water.svg" width="15px"/> Add `six_plus_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/six_minus.svg" width="15px"/> Add `six_minus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/six_plus.svg" width="15px"/> Add `six_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/roman_numeral_i_above_water.svg" width="15px"/> Add `roman_numeral_i_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/roman_numeral_ii_above_water.svg" width="15px"/> Add `roman_numeral_ii_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/roman_numeral_iii_above_water.svg" width="15px"/> Add `roman_numeral_iii_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/roman_numeral_iv_above_water.svg" width="15px"/> Add `roman_numeral_iv_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/roman_numeral_v_above_water.svg" width="15px"/> Add `roman_numeral_v_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/roman_numeral_vi_above_water.svg" width="15px"/> Add `roman_numeral_vi_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/x_above_water.svg" width="15px"/> Add `x_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/skull_above_water.svg" width="15px"/> Add `skull_above_water` by [@quincylvania](https://github.com/quincylvania) ([#200](https://github.com/waysidemapping/pinhead/issues/200))
- <img src="https://pinhead.ink/v24/p_wide_on_parking_line.svg" width="15px"/> Add `p_wide_on_parking_line` by [@quincylvania](https://github.com/quincylvania) ([#216](https://github.com/waysidemapping/pinhead/issues/216))
- <img src="https://pinhead.ink/v24/e_wide_on_parking_line.svg" width="15px"/> Add `e_wide_on_parking_line` by [@quincylvania](https://github.com/quincylvania) ([#216](https://github.com/waysidemapping/pinhead/issues/216))
- <img src="https://pinhead.ink/v24/p_wide_in_parking_structure.svg" width="15px"/> Add `p_wide_in_parking_structure` by [@quincylvania](https://github.com/quincylvania) ([#216](https://github.com/waysidemapping/pinhead/issues/216))
- <img src="https://pinhead.ink/v24/e_wide_in_parking_structure.svg" width="15px"/> Add `e_wide_in_parking_structure` by [@quincylvania](https://github.com/quincylvania) ([#216](https://github.com/waysidemapping/pinhead/issues/216))
- <img src="https://pinhead.ink/v24/p_wide_with_arrow_bottom_right.svg" width="15px"/> Add `p_wide_with_arrow_bottom_right` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/e_wide_with_arrow_bottom_right.svg" width="15px"/> Add `e_wide_with_arrow_bottom_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/p_wide_with_arrow_right.svg" width="15px"/> Add `p_wide_with_arrow_right` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/e_wide_with_arrow_right.svg" width="15px"/> Add `e_wide_with_arrow_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/p_wide_with_bicycle.svg" width="15px"/> Add `p_wide_with_bicycle` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/e_wide_with_bicycle.svg" width="15px"/> Add `e_wide_with_bicycle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_one_one_one.svg" width="15px"/> Add `phone_down_above_one_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_one_one_two.svg" width="15px"/> Add `phone_down_above_one_one_two` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_one_two_three.svg" width="15px"/> Add `phone_down_above_one_two_three` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_two_one_one.svg" width="15px"/> Add `phone_down_above_two_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_three_one_one.svg" width="15px"/> Add `phone_down_above_three_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_four_one_one.svg" width="15px"/> Add `phone_down_above_four_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_five_one_one.svg" width="15px"/> Add `phone_down_above_five_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_six_one_one.svg" width="15px"/> Add `phone_down_above_six_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_seven_one_one.svg" width="15px"/> Add `phone_down_above_seven_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_eight_one_one.svg" width="15px"/> Add `phone_down_above_eight_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_nine_one_one.svg" width="15px"/> Add `phone_down_above_nine_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_nine_eight_eight.svg" width="15px"/> Add `phone_down_above_nine_eight_eight` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/phone_down_above_nine_nine_nine.svg" width="15px"/> Add `phone_down_above_nine_nine_nine` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/left_bracket_and_cube.svg" width="15px"/> Add `left_bracket_and_cube` from [OSM Carto](https://github.com/openstreetmap-carto/openstreetmap-carto) imported by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/cube.svg" width="15px"/> Add `cube` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/saddle_shape.svg" width="15px"/> Add `saddle_shape` from [OSM Carto](https://github.com/openstreetmap-carto/openstreetmap-carto) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40), [#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/isosceles_trapezoid_tall_up.svg" width="15px"/> Add `isosceles_trapezoid_tall_up` by [@petercooperjr](https://github.com/petercooperjr), [@quincylvania](https://github.com/quincylvania) ([#104](https://github.com/waysidemapping/pinhead/issues/104))
- <img src="https://pinhead.ink/v24/isosceles_trapezoid_tall_down.svg" width="15px"/> Add `isosceles_trapezoid_tall_down` by [@petercooperjr](https://github.com/petercooperjr), [@quincylvania](https://github.com/quincylvania) ([#104](https://github.com/waysidemapping/pinhead/issues/104))
- <img src="https://pinhead.ink/v24/parallelogram_tall_right.svg" width="15px"/> Add `parallelogram_tall_right` by [@petercooperjr](https://github.com/petercooperjr), [@quincylvania](https://github.com/quincylvania) ([#104](https://github.com/waysidemapping/pinhead/issues/104))
- <img src="https://pinhead.ink/v24/parallelogram_tall_left.svg" width="15px"/> Add `parallelogram_tall_left` by [@petercooperjr](https://github.com/petercooperjr), [@quincylvania](https://github.com/quincylvania) ([#104](https://github.com/waysidemapping/pinhead/issues/104))
- <img src="https://pinhead.ink/v24/square_with_dot.svg" width="15px"/> Add `square_with_dot` by [@quincylvania](https://github.com/quincylvania) ([#180](https://github.com/waysidemapping/pinhead/issues/180))
- <img src="https://pinhead.ink/v24/square_with_square_dot.svg" width="15px"/> Add `square_with_square_dot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/octagon_outline.svg" width="15px"/> Add `octagon_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/map_pin_outline_with_dot.svg" width="15px"/> Add `map_pin_outline_with_dot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_left_from_rectangle_tall_outline.svg" width="15px"/> Add `arrow_left_from_rectangle_tall_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_left_to_rectangle_tall_outline.svg" width="15px"/> Add `arrow_left_to_rectangle_tall_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_right_from_rectangle_tall_outline.svg" width="15px"/> Add `arrow_right_from_rectangle_tall_outline` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v24/arrow_right_to_rectangle_tall_outline.svg" width="15px"/> Add `arrow_right_to_rectangle_tall_outline` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v24/arrow_up_from_rectangle_outline.svg" width="15px"/> Add `arrow_up_from_rectangle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_down_from_rectangle_outline.svg" width="15px"/> Add `arrow_down_from_rectangle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_up_to_rectangle_outline.svg" width="15px"/> Add `arrow_up_to_rectangle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/arrow_down_to_rectangle_outline.svg" width="15px"/> Add `arrow_down_to_rectangle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/pixel_exclamation_point.svg" width="15px"/> Add `pixel_exclamation_point` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/pixel_question_mark.svg" width="15px"/> Add `pixel_question_mark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v24/pixel_gasoline_pump.svg" width="15px"/> Add `pixel_gasoline_pump` by [@quincylvania](https://github.com/quincylvania)


## [15.23.0] - 2026-04-28

_Pinhead v23_

This release contains new and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Redesigned icons

- <img src="https://pinhead.ink/v22/atm_text.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/atm_text.svg" width="15px"/> `atm_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/sos_text.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/sos_text.svg" width="15px"/> `sos_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/water.svg" width="15px"/> `water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/arrows_left_right_above_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/arrows_left_right_above_water.svg" width="15px"/> `arrows_left_right_above_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/fountain_from_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/fountain_from_water.svg" width="15px"/> `fountain_from_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/waterfall_into_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/waterfall_into_water.svg" width="15px"/> `waterfall_into_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_swimming_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_swimming_in_water.svg" width="15px"/> `person_swimming_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_diving_into_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_diving_into_water.svg" width="15px"/> `person_diving_into_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_driving_motorboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_driving_motorboat_on_water.svg" width="15px"/> `person_driving_motorboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_riding_tube_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_riding_tube_on_water.svg" width="15px"/> `person_riding_tube_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_on_ground_dragging_raft_to_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_on_ground_dragging_raft_to_water.svg" width="15px"/> `person_on_ground_dragging_raft_to_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_fishing_from_pier_above_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_fishing_from_pier_above_water.svg" width="15px"/> `person_fishing_from_pier_above_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_in_water.svg" width="15px"/> `person_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_in_water_wearing_swim_briefs_holding_bucket.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_in_water_wearing_swim_briefs_holding_bucket.svg" width="15px"/> `person_in_water_wearing_swim_briefs_holding_bucket` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_in_water_with_steam.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_in_water_with_steam.svg" width="15px"/> `person_in_water_with_steam` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_paddling_canoe_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_paddling_canoe_on_water.svg" width="15px"/> `person_paddling_canoe_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_riding_jetski_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_riding_jetski_on_water.svg" width="15px"/> `person_riding_jetski_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_riding_pedal_boat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_riding_pedal_boat_on_water.svg" width="15px"/> `person_riding_pedal_boat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_rowing_rowboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_rowing_rowboat_on_water.svg" width="15px"/> `person_rowing_rowboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_sitting_on_lifeguard_stand_above_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_sitting_on_lifeguard_stand_above_water.svg" width="15px"/> `person_sitting_on_lifeguard_stand_above_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_tow_skiing_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_tow_skiing_on_water.svg" width="15px"/> `person_tow_skiing_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_wearing_helmet_padding_raft_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_wearing_helmet_padding_raft_on_water.svg" width="15px"/> `person_wearing_helmet_padding_raft_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_wearing_helmet_paddling_kayak_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_wearing_helmet_paddling_kayak_on_water.svg" width="15px"/> `person_wearing_helmet_paddling_kayak_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/person_wind_surfing_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/person_wind_surfing_on_water.svg" width="15px"/> `person_wind_surfing_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/broadleaved_tree_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/broadleaved_tree_in_water.svg" width="15px"/> `broadleaved_tree_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/grass_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/grass_in_water.svg" width="15px"/> `grass_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/typha_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/typha_in_water.svg" width="15px"/> `typha_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/watermill_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/watermill_on_water.svg" width="15px"/> `watermill_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/airboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/airboat_on_water.svg" width="15px"/> `airboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/cars_on_barge_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/cars_on_barge_on_water.svg" width="15px"/> `cars_on_barge_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/houseboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/houseboat_on_water.svg" width="15px"/> `houseboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/motorboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/motorboat_on_water.svg" width="15px"/> `motorboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/sailboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/sailboat_on_water.svg" width="15px"/> `sailboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/shipwreck_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/shipwreck_in_water.svg" width="15px"/> `shipwreck_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/tourboat_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/tourboat_on_water.svg" width="15px"/> `tourboat_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/seaplane_takeoff_over_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/seaplane_takeoff_over_water.svg" width="15px"/> `seaplane_takeoff_over_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/house_and_trees_on_hill_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/house_and_trees_on_hill_in_water.svg" width="15px"/> `house_and_trees_on_hill_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/tree_on_hill_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/tree_on_hill_in_water.svg" width="15px"/> `tree_on_hill_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/buoy_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/buoy_on_water.svg" width="15px"/> `buoy_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/pier_mounted_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/pier_mounted_in_water.svg" width="15px"/> `pier_mounted_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/pier_on_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/pier_on_water.svg" width="15px"/> `pier_on_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/rolled_paper_in_bottle_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/rolled_paper_in_bottle_in_water.svg" width="15px"/> `rolled_paper_in_bottle_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/duck_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/duck_in_water.svg" width="15px"/> `duck_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/typha_and_duck_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/typha_and_duck_in_water.svg" width="15px"/> `typha_and_duck_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/beaver_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/beaver_in_water.svg" width="15px"/> `beaver_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/whale_tail_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/whale_tail_in_water.svg" width="15px"/> `whale_tail_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/sailing_ship_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/sailing_ship_in_water.svg" width="15px"/> `sailing_ship_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v22/shark_dorsal_fin_in_waters.svg" width="15px"/> -> <img src="https://pinhead.ink/v23/shark_dorsal_fin_in_waters.svg" width="15px"/> `shark_dorsal_fin_in_waters` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))

### Added icons

- <img src="https://pinhead.ink/v23/navigation_arrow_up.svg" width="15px"/> Add `navigation_arrow_up` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/navigation_arrow_top_right.svg" width="15px"/> Add `navigation_arrow_top_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/kayak_beside_kayak_paddle.svg" width="15px"/> Add `kayak_beside_kayak_paddle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/kayak_paddle_crossing_kayak.svg" width="15px"/> Add `kayak_paddle_crossing_kayak` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/cot_campsite.svg" width="15px"/> Add `cot_campsite` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/cot_campsite_with_eyes.svg" width="15px"/> Add `cot_campsite_with_eyes` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/transit_vehicle.svg" width="15px"/> Add `transit_vehicle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/tram_on_tram_track.svg" width="15px"/> Add `tram_on_tram_track` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/tram_with_pantograph_on_tram_track.svg" width="15px"/> Add `tram_with_pantograph_on_tram_track` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/tram_with_destination_display_on_tram_track.svg" width="15px"/> Add `tram_with_destination_display_on_tram_track` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/club_chair.svg" width="15px"/> Add `club_chair` from [NPS](https://github.com/nationalparkservice/symbol-library) imported by [@quincylvania](https://github.com/quincylvania) ([#182](https://github.com/waysidemapping/pinhead/issues/182))
- <img src="https://pinhead.ink/v23/corn_cob.svg" width="15px"/> Add `corn_cob` by [@ooosssay](https://github.com/ooosssay) ([#201](https://github.com/waysidemapping/pinhead/issues/201), [#118](https://github.com/waysidemapping/pinhead/issues/118))
- <img src="https://pinhead.ink/v23/cheese_wedge.svg" width="15px"/> Add `cheese_wedge` by [@ooosssay](https://github.com/ooosssay) ([#203](https://github.com/waysidemapping/pinhead/issues/203), [#28](https://github.com/waysidemapping/pinhead/issues/28))
- <img src="https://pinhead.ink/v23/person_wearing_cheese_wedge_hat.svg" width="15px"/> Add `person_wearing_cheese_wedge_hat` by [@quincylvania](https://github.com/quincylvania) ([#113](https://github.com/waysidemapping/pinhead/issues/113))
- <img src="https://pinhead.ink/v23/lotus_flower.svg" width="15px"/> Add `lotus_flower` by [@ooosssay](https://github.com/ooosssay) ([#210](https://github.com/waysidemapping/pinhead/issues/210))
- <img src="https://pinhead.ink/v23/ankh.svg" width="15px"/> Add `ankh` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/confucian_bell.svg" width="15px"/> Add `confucian_bell` by [@ooosssay](https://github.com/ooosssay) ([#209](https://github.com/waysidemapping/pinhead/issues/209))
- <img src="https://pinhead.ink/v23/lu_zi_symbol.svg" width="15px"/> Add `lu_zi_symbol` by [@ooosssay](https://github.com/ooosssay) ([#208](https://github.com/waysidemapping/pinhead/issues/208))
- <img src="https://pinhead.ink/v23/pentagram_in_circle_outline.svg" width="15px"/> Add `pentagram_in_circle_outline` by [@ooosssay](https://github.com/ooosssay) ([#205](https://github.com/waysidemapping/pinhead/issues/205))
- <img src="https://pinhead.ink/v23/nine_point_star.svg" width="15px"/> Add `nine_point_star` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/nine_point_star_outline.svg" width="15px"/> Add `nine_point_star_outline` by [@ooosssay](https://github.com/ooosssay) ([#206](https://github.com/waysidemapping/pinhead/issues/206))
- <img src="https://pinhead.ink/v23/bulbed_star.svg" width="15px"/> Add `bulbed_star` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/faravahar.svg" width="15px"/> Add `faravahar` by [@ooosssay](https://github.com/ooosssay) ([#202](https://github.com/waysidemapping/pinhead/issues/202))
- <img src="https://pinhead.ink/v23/book_with_arrows_recirculating.svg" width="15px"/> Add `book_with_arrows_recirculating` by [@ooosssay](https://github.com/ooosssay)
- <img src="https://pinhead.ink/v23/book_with_balance_scales.svg" width="15px"/> Add `book_with_balance_scales` by [@ooosssay](https://github.com/ooosssay)
- <img src="https://pinhead.ink/v23/book_with_dna.svg" width="15px"/> Add `book_with_dna` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_info_i.svg" width="15px"/> Add `book_with_info_i` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_molar_tooth.svg" width="15px"/> Add `book_with_molar_tooth` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_music_notes_eighth.svg" width="15px"/> Add `book_with_music_notes_eighth` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_pawprint.svg" width="15px"/> Add `book_with_pawprint` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_pencil_and_apple.svg" width="15px"/> Add `book_with_pencil_and_apple` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_rocketship.svg" width="15px"/> Add `book_with_rocketship` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/book_with_square_academic_cap.svg" width="15px"/> Add `book_with_square_academic_cap` by [@ooosssay](https://github.com/ooosssay) ([#196](https://github.com/waysidemapping/pinhead/issues/196))
- <img src="https://pinhead.ink/v23/wc_text.svg" width="15px"/> Add `wc_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/arrows_left_right.svg" width="15px"/> Add `arrows_left_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/waters.svg" width="15px"/> Add `waters` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/person_swimming_in_waters.svg" width="15px"/> Add `person_swimming_in_waters` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/seaplane_takeoff.svg" width="15px"/> Add `seaplane_takeoff` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/whale_tail.svg" width="15px"/> Add `whale_tail` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/sailing_ship.svg" width="15px"/> Add `sailing_ship` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v23/shark_dorsal_fin_in_water.svg" width="15px"/> Add `shark_dorsal_fin_in_water` by [@quincylvania](https://github.com/quincylvania) ([#135](https://github.com/waysidemapping/pinhead/issues/135))
- <img src="https://pinhead.ink/v23/person_walking_in_water.svg" width="15px"/> Add `person_walking_in_water` by [@quincylvania](https://github.com/quincylvania) ([#94](https://github.com/waysidemapping/pinhead/issues/94))
- <img src="https://pinhead.ink/v23/person_walking_in_waters.svg" width="15px"/> Add `person_walking_in_waters` by [@quincylvania](https://github.com/quincylvania) ([#95](https://github.com/waysidemapping/pinhead/issues/95))

## [15.22.0] - 2026-04-15

_Pinhead v22_

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v21/parking_p.svg" width="15px"/> `parking_p` -> <img src="https://pinhead.ink/v22/p_wide.svg" width="15px"/> `p_wide` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/parking_p_with_parking_meter.svg" width="15px"/> `parking_p_with_parking_meter` -> <img src="https://pinhead.ink/v22/p_wide_with_parking_meter.svg" width="15px"/> `p_wide_with_parking_meter` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/parking_p_under_roof.svg" width="15px"/> `parking_p_under_roof` -> <img src="https://pinhead.ink/v22/p_wide_under_roof.svg" width="15px"/> `p_wide_under_roof` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/phone_and_keyboard.svg" width="15px"/> `phone_and_keyboard` -> <img src="https://pinhead.ink/v22/phone_down_above_keyboard.svg" width="15px"/> `phone_down_above_keyboard` by [@quincylvania](https://github.com/quincylvania)

### Redesigned icons

- <img src="https://pinhead.ink/v21/fork_and_knife.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/fork_and_knife.svg" width="15px"/> `fork_and_knife` by [@westnordost](https://github.com/westnordost) ([#183](https://github.com/waysidemapping/pinhead/issues/183))
- <img src="https://pinhead.ink/v21/fork_and_spoon.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/fork_and_spoon.svg" width="15px"/> `fork_and_spoon` by [@westnordost](https://github.com/westnordost) ([#183](https://github.com/waysidemapping/pinhead/issues/183))
- <img src="https://pinhead.ink/v21/spoon_and_fork.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/spoon_and_fork.svg" width="15px"/> `spoon_and_fork` by [@westnordost](https://github.com/westnordost) ([#183](https://github.com/waysidemapping/pinhead/issues/183))
- <img src="https://pinhead.ink/v21/fork_and_sausage.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/fork_and_sausage.svg" width="15px"/> `fork_and_sausage` by [@westnordost](https://github.com/westnordost) ([#183](https://github.com/waysidemapping/pinhead/issues/183))
- <img src="https://pinhead.ink/v21/calculator.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/calculator.svg" width="15px"/> `calculator` by [@westnordost](https://github.com/westnordost) ([#183](https://github.com/waysidemapping/pinhead/issues/183))
- <img src="https://pinhead.ink/v21/crates_under_roof.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/crates_under_roof.svg" width="15px"/> `crates_under_roof` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/x.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/x.svg" width="15px"/> `x` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v21/phone_top_right_with_greek_cross.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/phone_top_right_with_greek_cross.svg" width="15px"/> `phone_top_right_with_greek_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/phone_right_with_exclamation_point.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/phone_right_with_exclamation_point.svg" width="15px"/> `phone_right_with_exclamation_point` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/phone_bottom_right.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/phone_bottom_right.svg" width="15px"/> `phone_bottom_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/person_sitting_in_seat.svg" width="15px"/> -> <img src="https://pinhead.ink/v22/person_sitting_in_seat.svg" width="15px"/> `person_sitting_in_seat` by [@quincylvania](https://github.com/quincylvania) ([#194](https://github.com/waysidemapping/pinhead/issues/194))

### Added icons

- <img src="https://pinhead.ink/v22/triangles_up_down_in_rectangle_outline.svg" width="15px"/> Add `triangles_up_down_in_rectangle_outline` by [@quincylvania](https://github.com/quincylvania) ([##40](https://github.com/waysidemapping/pinhead/issues/#40))
- <img src="https://pinhead.ink/v22/triangles_left_right_in_rectangle_outline.svg" width="15px"/> Add `triangles_left_right_in_rectangle_outline` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/gumdrop_head_and_shoulders.svg" width="15px"/> Add `gumdrop_head_and_shoulders` by [@quincylvania](https://github.com/quincylvania) ([#49](https://github.com/waysidemapping/pinhead/issues/49))
- <img src="https://pinhead.ink/v22/head_and_shoulders.svg" width="15px"/> Add `head_and_shoulders` by [@quincylvania](https://github.com/quincylvania) ([#49](https://github.com/waysidemapping/pinhead/issues/49))
- <img src="https://pinhead.ink/v22/pixel_head_and_shoulders.svg" width="15px"/> Add `pixel_head_and_shoulders` by [@quincylvania](https://github.com/quincylvania) ([#49](https://github.com/waysidemapping/pinhead/issues/49))
- <img src="https://pinhead.ink/v22/flying_saucer.svg" width="15px"/> Add `flying_saucer` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/spooky_ghost.svg" width="15px"/> Add `spooky_ghost` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/poultry_drumstick.svg" width="15px"/> Add `poultry_drumstick` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185), [#23](https://github.com/waysidemapping/pinhead/issues/23))
- <img src="https://pinhead.ink/v22/chip_bag.svg" width="15px"/> Add `chip_bag` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/chip_bag_with_chip.svg" width="15px"/> Add `chip_bag_with_chip` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/conifer_tree_with_star_and_ornaments.svg" width="15px"/> Add `conifer_tree_with_star_and_ornaments` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/two_button_computer_mouse_with_scroll_wheel.svg" width="15px"/> Add `two_button_computer_mouse_with_scroll_wheel` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/puzzle_piece.svg" width="15px"/> Add `puzzle_piece` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185), [#33](https://github.com/waysidemapping/pinhead/issues/33))
- <img src="https://pinhead.ink/v22/confetti_ball.svg" width="15px"/> Add `confetti_ball` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/party_popper.svg" width="15px"/> Add `party_popper` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/shooting_stars.svg" width="15px"/> Add `shooting_stars` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/trophy.svg" width="15px"/> Add `trophy` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/trophy_with_star.svg" width="15px"/> Add `trophy_with_star` by [@ooosssay](https://github.com/ooosssay) ([#185](https://github.com/waysidemapping/pinhead/issues/185))
- <img src="https://pinhead.ink/v22/banana.svg" width="15px"/> Add `banana` by [@ooosssay](https://github.com/ooosssay) ([#186](https://github.com/waysidemapping/pinhead/issues/186), [#35](https://github.com/waysidemapping/pinhead/issues/35))
- <img src="https://pinhead.ink/v22/banana_hand.svg" width="15px"/> Add `banana_hand` by [@ooosssay](https://github.com/ooosssay) ([#186](https://github.com/waysidemapping/pinhead/issues/186), [#35](https://github.com/waysidemapping/pinhead/issues/35))
- <img src="https://pinhead.ink/v22/banana_and_apple.svg" width="15px"/> Add `banana_and_apple` by [@ooosssay](https://github.com/ooosssay) ([#186](https://github.com/waysidemapping/pinhead/issues/186), [#35](https://github.com/waysidemapping/pinhead/issues/35))
- <img src="https://pinhead.ink/v22/hand_grenade.svg" width="15px"/> Add `hand_grenade` by [@ooosssay](https://github.com/ooosssay) ([#191](https://github.com/waysidemapping/pinhead/issues/191))
- <img src="https://pinhead.ink/v22/magic_wand_and_sparkles.svg" width="15px"/> Add `magic_wand_and_sparkles` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/baby_in_swaddle.svg" width="15px"/> Add `baby_in_swaddle` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/baby_crawling.svg" width="15px"/> Add `baby_crawling` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/person_holding_cane.svg" width="15px"/> Add `person_holding_cane` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/person_wearing_dress_holding_cane.svg" width="15px"/> Add `person_wearing_dress_holding_cane` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/hazmat_suit.svg" width="15px"/> Add `hazmat_suit` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/liver.svg" width="15px"/> Add `liver` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/liver_with_bile_duct.svg" width="15px"/> Add `liver_with_bile_duct` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/spinal_vertebrae.svg" width="15px"/> Add `spinal_vertebrae` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/spherical_virus.svg" width="15px"/> Add `spherical_virus` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/bathroom_scale.svg" width="15px"/> Add `bathroom_scale` from [Health Icons](https://github.com/resolvetosavelives/healthicons) imported by [@quincylvania](https://github.com/quincylvania) ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v22/a.svg" width="15px"/> Add `a` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/b.svg" width="15px"/> Add `b` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/c.svg" width="15px"/> Add `c` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/d.svg" width="15px"/> Add `d` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/e.svg" width="15px"/> Add `e` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/e_wide.svg" width="15px"/> Add `e_wide` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/e_wide_with_parking_meter.svg" width="15px"/> Add `e_wide_with_parking_meter` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/parking_stall_markings_with_e_wide.svg" width="15px"/> Add `parking_stall_markings_with_e_wide` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/e_wide_under_roof.svg" width="15px"/> Add `e_wide_under_roof` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/f.svg" width="15px"/> Add `f` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/g.svg" width="15px"/> Add `g` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/h.svg" width="15px"/> Add `h` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/i.svg" width="15px"/> Add `i` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/j.svg" width="15px"/> Add `j` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/k.svg" width="15px"/> Add `k` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/l.svg" width="15px"/> Add `l` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/m.svg" width="15px"/> Add `m` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/n.svg" width="15px"/> Add `n` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/o.svg" width="15px"/> Add `o` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/p.svg" width="15px"/> Add `p` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/parking_stall_markings_with_p_wide.svg" width="15px"/> Add `parking_stall_markings_with_p_wide` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/q.svg" width="15px"/> Add `q` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/r.svg" width="15px"/> Add `r` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/s.svg" width="15px"/> Add `s` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/t.svg" width="15px"/> Add `t` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/u.svg" width="15px"/> Add `u` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/v.svg" width="15px"/> Add `v` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/w.svg" width="15px"/> Add `w` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/y.svg" width="15px"/> Add `y` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/z.svg" width="15px"/> Add `z` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/zero.svg" width="15px"/> Add `zero` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/zero_with_slash.svg" width="15px"/> Add `zero_with_slash` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/one.svg" width="15px"/> Add `one` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/two.svg" width="15px"/> Add `two` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/three.svg" width="15px"/> Add `three` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/four.svg" width="15px"/> Add `four` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/five.svg" width="15px"/> Add `five` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/six.svg" width="15px"/> Add `six` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/seven.svg" width="15px"/> Add `seven` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/eight.svg" width="15px"/> Add `eight` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/nine.svg" width="15px"/> Add `nine` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/ten.svg" width="15px"/> Add `ten` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/eleven.svg" width="15px"/> Add `eleven` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/twelve.svg" width="15px"/> Add `twelve` by [@quincylvania](https://github.com/quincylvania) ([#10](https://github.com/waysidemapping/pinhead/issues/10))
- <img src="https://pinhead.ink/v22/nine_one_one.svg" width="15px"/> Add `nine_one_one` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/atm_text.svg" width="15px"/> Add `atm_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/sos_text.svg" width="15px"/> Add `sos_text` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_top_right.svg" width="15px"/> Add `phone_top_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_top_right_with_plus.svg" width="15px"/> Add `phone_top_right_with_plus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_right.svg" width="15px"/> Add `phone_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_right_with_beams_from_receiver.svg" width="15px"/> Add `phone_right_with_beams_from_receiver` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_down.svg" width="15px"/> Add `phone_down` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v22/phone_down_above_sos_text.svg" width="15px"/> Add `phone_down_above_sos_text` by [@quincylvania](https://github.com/quincylvania)


## [15.21.0] - 2026-03-29

_Pinhead v21_

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v20/vending_machine.svg" width="15px"/> `vending_machine` -> <img src="https://pinhead.ink/v21/vending_machine_with_shelves.svg" width="15px"/> `vending_machine_with_shelves` by [@quincylvania](https://github.com/quincylvania)

### Renamed icons

- <img src="https://pinhead.ink/v21/budded_latin_cross.svg" width="15px"/> `greek_orthodox_cross` -> `budded_latin_cross`

### Redesigned icons

- <img src="https://pinhead.ink/v20/typha_and_duck_in_water.svg" width="15px"/> -> <img src="https://pinhead.ink/v21/typha_and_duck_in_water.svg" width="15px"/> `typha_and_duck_in_water` by [@ooosssay](https://github.com/ooosssay) ([#168](https://github.com/waysidemapping/pinhead/issues/168))
- <img src="https://pinhead.ink/v20/book.svg" width="15px"/> -> <img src="https://pinhead.ink/v21/book.svg" width="15px"/> `book` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/meat.svg" width="15px"/> -> <img src="https://pinhead.ink/v21/meat.svg" width="15px"/> `meat` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))

### Added icons

- <img src="https://pinhead.ink/v21/taco.svg" width="15px"/> Add `taco` by [@ooosssay](https://github.com/ooosssay) ([#178](https://github.com/waysidemapping/pinhead/issues/178))
- <img src="https://pinhead.ink/v21/pretzel_with_salt.svg" width="15px"/> Add `pretzel_with_salt` from [source](https://raw.githubusercontent.com/twain47/Open-SVG-Map-Icons/refs/heads/master/svg/shopping/bakery.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#179](https://github.com/waysidemapping/pinhead/issues/179), [#21](https://github.com/waysidemapping/pinhead/issues/21))
- <img src="https://pinhead.ink/v21/oak_leaf.svg" width="15px"/> Add `oak_leaf` by [@ooosssay](https://github.com/ooosssay) ([#179](https://github.com/waysidemapping/pinhead/issues/179), [#22](https://github.com/waysidemapping/pinhead/issues/22))
- <img src="https://pinhead.ink/v21/chopsticks.svg" width="15px"/> Add `chopsticks` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#174](https://github.com/waysidemapping/pinhead/issues/174))
- <img src="https://pinhead.ink/v21/chopsticks_crossed.svg" width="15px"/> Add `chopsticks_crossed` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/spoon_and_chopsticks.svg" width="15px"/> Add `spoon_and_chopsticks` by [@ooosssay](https://github.com/ooosssay) ([#174](https://github.com/waysidemapping/pinhead/issues/174))
- <img src="https://pinhead.ink/v21/spoon_and_fork.svg" width="15px"/> Add `spoon_and_fork` by [@ooosssay](https://github.com/ooosssay) ([#174](https://github.com/waysidemapping/pinhead/issues/174))
- <img src="https://pinhead.ink/v21/fork_and_spoon.svg" width="15px"/> Add `fork_and_spoon` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/drink_can.svg" width="15px"/> Add `drink_can` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/whistle.svg" width="15px"/> Add `whistle` by [@ooosssay](https://github.com/ooosssay) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/pawprint_and_whistle.svg" width="15px"/> Add `pawprint_and_whistle` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/dog_sitting_wearing_collar_and_whistle.svg" width="15px"/> Add `dog_sitting_wearing_collar_and_whistle` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/dog_sitting_wearing_harness_and_whistle.svg" width="15px"/> Add `dog_sitting_wearing_harness_and_whistle` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/dog_sitting_wearing_collar_and_heart.svg" width="15px"/> Add `dog_sitting_wearing_collar_and_heart` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/pawprints_and_heart.svg" width="15px"/> Add `pawprints_and_heart` by [@ooosssay](https://github.com/ooosssay) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/shopping_bag_with_pawprint.svg" width="15px"/> Add `shopping_bag_with_pawprint` by [@ooosssay](https://github.com/ooosssay) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/cup_and_saucer_and_pawprint.svg" width="15px"/> Add `cup_and_saucer_and_pawprint` by [@ooosssay](https://github.com/ooosssay) ([#170](https://github.com/waysidemapping/pinhead/issues/170))
- <img src="https://pinhead.ink/v21/duck_in_water.svg" width="15px"/> Add `duck_in_water` by [@ooosssay](https://github.com/ooosssay) ([#168](https://github.com/waysidemapping/pinhead/issues/168))
- <img src="https://pinhead.ink/v21/duck.svg" width="15px"/> Add `duck` by [@ooosssay](https://github.com/ooosssay) ([#168](https://github.com/waysidemapping/pinhead/issues/168))
- <img src="https://pinhead.ink/v21/typha_in_water.svg" width="15px"/> Add `typha_in_water` by [@ooosssay](https://github.com/ooosssay) ([#168](https://github.com/waysidemapping/pinhead/issues/168))
- <img src="https://pinhead.ink/v21/anime_eye_and_eyebrow.svg" width="15px"/> Add `anime_eye_and_eyebrow` by [@ooosssay](https://github.com/ooosssay) ([#171](https://github.com/waysidemapping/pinhead/issues/171))
- <img src="https://pinhead.ink/v21/shopping_bag_with_anime_eye_and_eyebrow.svg" width="15px"/> Add `shopping_bag_with_anime_eye_and_eyebrow` by [@ooosssay](https://github.com/ooosssay) ([#171](https://github.com/waysidemapping/pinhead/issues/171))
- <img src="https://pinhead.ink/v21/ichthys.svg" width="15px"/> Add `ichthys` by [@quincylvania](https://github.com/quincylvania) ([#177](https://github.com/waysidemapping/pinhead/issues/177))
- <img src="https://pinhead.ink/v21/book_with_bookmark.svg" width="15px"/> Add `book_with_bookmark` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/book_with_bookmark_in_slot.svg" width="15px"/> Add `book_with_bookmark_in_slot` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#172](https://github.com/waysidemapping/pinhead/issues/172))
- <img src="https://pinhead.ink/v21/arrow_down_from_book_with_bookmark_in_slot.svg" width="15px"/> Add `arrow_down_from_book_with_bookmark_in_slot` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#172](https://github.com/waysidemapping/pinhead/issues/172))
- <img src="https://pinhead.ink/v21/arrow_up_to_book_with_bookmark_in_slot.svg" width="15px"/> Add `arrow_up_to_book_with_bookmark_in_slot` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#172](https://github.com/waysidemapping/pinhead/issues/172))
- <img src="https://pinhead.ink/v21/pen_nib.svg" width="15px"/> Add `pen_nib` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/oval_broadleaved_tree.svg" width="15px"/> Add `oval_broadleaved_tree` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/conifer_tree_and_oval_broadleaved_tree.svg" width="15px"/> Add `conifer_tree_and_oval_broadleaved_tree` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/three_books_stacked.svg" width="15px"/> Add `three_books_stacked` from [Osmic](https://github.com/gmgeo/osmic) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/shaker_pint_glass.svg" width="15px"/> Add `shaker_pint_glass` from [OSM Carto](https://github.com/openstreetmap-carto/openstreetmap-carto) imported by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/transit_vehicle_on_railway_track_in_tunnel.svg" width="15px"/> Add `transit_vehicle_on_railway_track_in_tunnel` by [@quincylvania](https://github.com/quincylvania) ([#40](https://github.com/waysidemapping/pinhead/issues/40))
- <img src="https://pinhead.ink/v21/vending_machine.svg" width="15px"/> Add `vending_machine` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v21/vending_machine_with_baguette.svg" width="15px"/> Add `vending_machine_with_baguette` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_egg.svg" width="15px"/> Add `vending_machine_with_egg` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_cigarette_with_smoke_curl.svg" width="15px"/> Add `vending_machine_with_cigarette_with_smoke_curl` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_drink_can.svg" width="15px"/> Add `vending_machine_with_drink_can` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_drink_cup_with_steam.svg" width="15px"/> Add `vending_machine_with_drink_cup_with_steam` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_ice_cream_on_cone.svg" width="15px"/> Add `vending_machine_with_ice_cream_on_cone` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_heart.svg" width="15px"/> Add `vending_machine_with_heart` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_greek_cross.svg" width="15px"/> Add `vending_machine_with_greek_cross` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_postage_stamp.svg" width="15px"/> Add `vending_machine_with_postage_stamp` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_ticket.svg" width="15px"/> Add `vending_machine_with_ticket` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))
- <img src="https://pinhead.ink/v21/vending_machine_with_venus.svg" width="15px"/> Add `vending_machine_with_venus` by [@quincylvania](https://github.com/quincylvania) ([#181](https://github.com/waysidemapping/pinhead/issues/181))


## [15.20.0] - 2026-03-25

_Pinhead v20_

This release contains new and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Distribution changes

- The QGIS plugin has been dropped in favor of a repository compatible with the QGIS Resoure Sharing plugin:
  - https://github.com/waysidemapping/pinhead-qgis-resources
- Pinhead is now distributed as a web font:
  - Versioned Node package:
    - https://www.npmjs.com/@waysidemapping/pinhead-font
  - Hosted files per version:
    - https://pinhead.ink/v20/pinhead.ttf
    - https://pinhead.ink/v20/pinhead.css
    - https://pinhead.ink/v20/font_preview.html

### Redesigned icons

- <img src="https://pinhead.ink/v19/shopping_bag.svg" width="15px"/> -> <img src="https://pinhead.ink/v20/shopping_bag.svg" width="15px"/> `shopping_bag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/latin_cross.svg" width="15px"/> -> <img src="https://pinhead.ink/v20/latin_cross.svg" width="15px"/> `latin_cross` by [@quincylvania](https://github.com/quincylvania)

### Added icons

- <img src="https://pinhead.ink/v20/person_wearing_seatbelt.svg" width="15px"/> Add `person_wearing_seatbelt` by [@ooosssay](https://github.com/ooosssay) ([#161](https://github.com/waysidemapping/pinhead/issues/161), [#37](https://github.com/waysidemapping/pinhead/issues/37))
- <img src="https://pinhead.ink/v20/passport_with_belgium.svg" width="15px"/> Add `passport_with_belgium` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v20/passport_with_netherlands.svg" width="15px"/> Add `passport_with_netherlands` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v20/passport_with_bundesadler.svg" width="15px"/> Add `passport_with_bundesadler` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v20/graticule_globe.svg" width="15px"/> Add `graticule_globe` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/four_square_court.svg" width="15px"/> Add `four_square_court` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#162](https://github.com/waysidemapping/pinhead/issues/162))
- <img src="https://pinhead.ink/v20/four_square_court_with_ball.svg" width="15px"/> Add `four_square_court_with_ball` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania) ([#162](https://github.com/waysidemapping/pinhead/issues/162))
- <img src="https://pinhead.ink/v20/circle_a.svg" width="15px"/> Add `circle_a` by [@ooosssay](https://github.com/ooosssay) ([#163](https://github.com/waysidemapping/pinhead/issues/163))
- <img src="https://pinhead.ink/v20/tags.svg" width="15px"/> Add `tags` by [@quincylvania](https://github.com/quincylvania)

Add boundary icons:

- <img src="https://pinhead.ink/v20/africa.svg" width="15px"/> Add `africa` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/africa_and_madagascar.svg" width="15px"/> Add `africa_and_madagascar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/madagascar.svg" width="15px"/> Add `madagascar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/madagascar_with_capital_star.svg" width="15px"/> Add `madagascar_with_capital_star` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/belgium.svg" width="15px"/> Add `belgium` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/belgium_with_capital_star.svg" width="15px"/> Add `belgium_with_capital_star` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/netherlands.svg" width="15px"/> Add `netherlands` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/netherlands_with_capital_star.svg" width="15px"/> Add `netherlands_with_capital_star` by [@quincylvania](https://github.com/quincylvania)

Add shopping bag icons:

- <img src="https://pinhead.ink/v20/shopping_bag_with_dollar.svg" width="15px"/> Add `shopping_bag_with_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_arrows_recirculating.svg" width="15px"/> Add `shopping_bag_with_arrows_recirculating` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_euro.svg" width="15px"/> Add `shopping_bag_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_pound.svg" width="15px"/> Add `shopping_bag_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_yen_yuan.svg" width="15px"/> Add `shopping_bag_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_rupee.svg" width="15px"/> Add `shopping_bag_with_rupee` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/shopping_bag_with_ruble.svg" width="15px"/> Add `shopping_bag_with_ruble` by [@quincylvania](https://github.com/quincylvania)

Add Philippine peso icons:

- <img src="https://pinhead.ink/v20/peso.svg" width="15px"/> Add `peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/person_using_terminal_kiosk_with_peso.svg" width="15px"/> Add `person_using_terminal_kiosk_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/milk_carton_and_apple_and_peso.svg" width="15px"/> Add `milk_carton_and_apple_and_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/shopping_bag_with_peso.svg" width="15px"/> Add `shopping_bag_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/car_with_peso.svg" width="15px"/> Add `car_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/cargobike_and_peso.svg" width="15px"/> Add `cargobike_and_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/bicycle_and_peso.svg" width="15px"/> Add `bicycle_and_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/tag_with_peso.svg" width="15px"/> Add `tag_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/campsite_with_peso.svg" width="15px"/> Add `campsite_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))
- <img src="https://pinhead.ink/v20/tipi_campsite_with_peso.svg" width="15px"/> Add `tipi_campsite_with_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156))

Add religious icons:

- <img src="https://pinhead.ink/v20/star_of_david_with_dot.svg" width="15px"/> Add `star_of_david_with_dot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/nordic_cross.svg" width="15px"/> Add `nordic_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/petrine_cross.svg" width="15px"/> Add `petrine_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/saint_georges_cross.svg" width="15px"/> Add `saint_georges_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/patriarchal_cross.svg" width="15px"/> Add `patriarchal_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/papal_cross.svg" width="15px"/> Add `papal_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/russian_orthodox_cross.svg" width="15px"/> Add `russian_orthodox_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/russian_cross.svg" width="15px"/> Add `russian_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/celtic_cross.svg" width="15px"/> Add `celtic_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/greek_orthodox_cross.svg" width="15px"/> Add `greek_orthodox_cross` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/angel_moroni.svg" width="15px"/> Add `angel_moroni` by [@ooosssay](https://github.com/ooosssay) ([#166](https://github.com/waysidemapping/pinhead/issues/166))
- <img src="https://pinhead.ink/v20/spiral_labyrinth.svg" width="15px"/> Add `spiral_labyrinth` by [@quincylvania](https://github.com/quincylvania) ([#73](https://github.com/waysidemapping/pinhead/issues/73))
- <img src="https://pinhead.ink/v20/circular_labyrinth.svg" width="15px"/> Add `circular_labyrinth` by [@quincylvania](https://github.com/quincylvania) ([#73](https://github.com/waysidemapping/pinhead/issues/73))
- <img src="https://pinhead.ink/v20/ahimsa_hand_outline.svg" width="15px"/> Add `ahimsa_hand_outline` by [@ooosssay](https://github.com/ooosssay) ([#166](https://github.com/waysidemapping/pinhead/issues/166))
- <img src="https://pinhead.ink/v20/sauvastika.svg" width="15px"/> Add `sauvastika` by [@ooosssay](https://github.com/ooosssay) ([#163](https://github.com/waysidemapping/pinhead/issues/163))
- <img src="https://pinhead.ink/v20/sauvastika_with_dots.svg" width="15px"/> Add `sauvastika_with_dots` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/swastika.svg" width="15px"/> Add `swastika` by [@ooosssay](https://github.com/ooosssay) ([#163](https://github.com/waysidemapping/pinhead/issues/163))
- <img src="https://pinhead.ink/v20/swastika_with_dots.svg" width="15px"/> Add `swastika_with_dots` by [@ooosssay](https://github.com/ooosssay), [@quincylvania](https://github.com/quincylvania)

Add pixel icons:

- <img src="https://pinhead.ink/v20/pixel_peso.svg" width="15px"/> Add `pixel_peso` by [@quincylvania](https://github.com/quincylvania) ([#156](https://github.com/waysidemapping/pinhead/issues/156), [#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_dollar.svg" width="15px"/> Add `pixel_dollar` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_euro.svg" width="15px"/> Add `pixel_euro` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_pound.svg" width="15px"/> Add `pixel_pound` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_yen_yuan.svg" width="15px"/> Add `pixel_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_rupee.svg" width="15px"/> Add `pixel_rupee` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_ruble.svg" width="15px"/> Add `pixel_ruble` by [@quincylvania](https://github.com/quincylvania) ([#159](https://github.com/waysidemapping/pinhead/issues/159))
- <img src="https://pinhead.ink/v20/pixel_droplet.svg" width="15px"/> Add `pixel_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_droplet_with_shine.svg" width="15px"/> Add `pixel_droplet_with_shine` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_envelope.svg" width="15px"/> Add `pixel_envelope` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_burger_on_bun.svg" width="15px"/> Add `pixel_burger_on_bun` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_burger_with_cheese_on_bun.svg" width="15px"/> Add `pixel_burger_with_cheese_on_bun` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_burger_on_bun_with_seeds.svg" width="15px"/> Add `pixel_burger_on_bun_with_seeds` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_burger_with_cheese_on_bun_with_seeds.svg" width="15px"/> Add `pixel_burger_with_cheese_on_bun_with_seeds` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_bicycle.svg" width="15px"/> Add `pixel_bicycle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_car.svg" width="15px"/> Add `pixel_car` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_taxi.svg" width="15px"/> Add `pixel_taxi` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_bus.svg" width="15px"/> Add `pixel_bus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v20/pixel_transit_vehicle_on_railway_track.svg" width="15px"/> Add `pixel_transit_vehicle_on_railway_track` by [@quincylvania](https://github.com/quincylvania)

## [15.19.0] - 2026-03-22

_Pinhead v19_

### Redesigned icons

- <img src="https://pinhead.ink/v18/dollar_swap_to_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/dollar_swap_to_euro.svg" width="15px"/> `dollar_swap_to_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/euro.svg" width="15px"/> `euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/yen_yuan.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/yen_yuan.svg" width="15px"/> `yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v18/campsite_with_dollar.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/campsite_with_dollar.svg" width="15px"/> `campsite_with_dollar` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/campsite_with_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/campsite_with_euro.svg" width="15px"/> `campsite_with_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/tipi_campsite_with_dollar.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/tipi_campsite_with_dollar.svg" width="15px"/> `tipi_campsite_with_dollar` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/tipi_campsite_with_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/tipi_campsite_with_euro.svg" width="15px"/> `tipi_campsite_with_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/bicycle_and_dollar.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/bicycle_and_dollar.svg" width="15px"/> `bicycle_and_dollar` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/bicycle_and_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/bicycle_and_euro.svg" width="15px"/> `bicycle_and_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/cargobike_and_dollar.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/cargobike_and_dollar.svg" width="15px"/> `cargobike_and_dollar` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/cargobike_and_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/cargobike_and_euro.svg" width="15px"/> `cargobike_and_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/car_with_dollar.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/car_with_dollar.svg" width="15px"/> `car_with_dollar` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/car_with_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/car_with_euro.svg" width="15px"/> `car_with_euro` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/milk_carton_and_apple_and_euro.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_euro.svg" width="15px"/> `milk_carton_and_apple_and_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/noodle_bowl_and_chopsticks_with_noodles.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/noodle_bowl_and_chopsticks_with_noodles.svg" width="15px"/> `noodle_bowl_and_chopsticks_with_noodles` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/paint_roller.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/paint_roller.svg" width="15px"/> `paint_roller` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/person_behind_barred_window.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/person_behind_barred_window.svg" width="15px"/> `person_behind_barred_window` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/terminal_screen_with_dollar_prompt.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/terminal_screen_with_dollar_prompt.svg" width="15px"/> `terminal_screen_with_dollar_prompt` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/boxes_on_pallet.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/boxes_on_pallet.svg" width="15px"/> `boxes_on_pallet` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/life_ring.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/life_ring.svg" width="15px"/> `life_ring` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/soccer_ball.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/soccer_ball.svg" width="15px"/> `soccer_ball` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/target.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/target.svg" width="15px"/> `target` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v18/target_with_archery_arrow_at_bullseye.svg" width="15px"/> -> <img src="https://pinhead.ink/v19/target_with_archery_arrow_at_bullseye.svg" width="15px"/> `target_with_archery_arrow_at_bullseye` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))

### Added icons

- <img src="https://pinhead.ink/v19/crosshair.svg" width="15px"/> Add `crosshair` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v19/bench_with_armrests.svg" width="15px"/> Add `bench_with_armrests` by [@quincylvania](https://github.com/quincylvania) ([#148](https://github.com/waysidemapping/pinhead/issues/148))
- <img src="https://pinhead.ink/v19/bench_with_armrests_and_backrest.svg" width="15px"/> Add `bench_with_armrests_and_backrest` by [@quincylvania](https://github.com/quincylvania) ([#148](https://github.com/waysidemapping/pinhead/issues/148))
- <img src="https://pinhead.ink/v19/person_sitting_on_bench.svg" width="15px"/> Add `person_sitting_on_bench` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/person_sitting_on_bench_with_armrests.svg" width="15px"/> Add `person_sitting_on_bench_with_armrests` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/person_sitting_on_bench_with_backrest.svg" width="15px"/> Add `person_sitting_on_bench_with_backrest` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/person_sitting_on_bench_with_armrests_and_backrest.svg" width="15px"/> Add `person_sitting_on_bench_with_armrests_and_backrest` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/bench_with_plaque.svg" width="15px"/> Add `bench_with_plaque` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/bench_with_plaque_and_armrests.svg" width="15px"/> Add `bench_with_plaque_and_armrests` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/bench_with_backrest_with_plaque.svg" width="15px"/> Add `bench_with_backrest_with_plaque` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/bench_with_armrests_and_backrest_with_plaque.svg" width="15px"/> Add `bench_with_armrests_and_backrest_with_plaque` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/dog_sitting.svg" width="15px"/> Add `dog_sitting` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_and_exclamation_point.svg" width="15px"/> Add `dog_sitting_and_exclamation_point` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_wearing_collar.svg" width="15px"/> Add `dog_sitting_wearing_collar` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_wearing_collar_and_exclamation_point.svg" width="15px"/> Add `dog_sitting_wearing_collar_and_exclamation_point` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_wearing_collar_on_leash.svg" width="15px"/> Add `dog_sitting_wearing_collar_on_leash` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_wearing_harness.svg" width="15px"/> Add `dog_sitting_wearing_harness` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/dog_sitting_wearing_harness_on_leash.svg" width="15px"/> Add `dog_sitting_wearing_harness_on_leash` by [@quincylvania](https://github.com/quincylvania) ([#149](https://github.com/waysidemapping/pinhead/issues/149))
- <img src="https://pinhead.ink/v19/rupee.svg" width="15px"/> Add `rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/ruble.svg" width="15px"/> Add `ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/tag_with_dollar.svg" width="15px"/> Add `tag_with_dollar` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150))
- <img src="https://pinhead.ink/v19/tag_with_euro.svg" width="15px"/> Add `tag_with_euro` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150))
- <img src="https://pinhead.ink/v19/tag_with_pound.svg" width="15px"/> Add `tag_with_pound` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150))
- <img src="https://pinhead.ink/v19/tag_with_yen_yuan.svg" width="15px"/> Add `tag_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150), [#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/tag_with_rupee.svg" width="15px"/> Add `tag_with_rupee` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150), [#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/tag_with_ruble.svg" width="15px"/> Add `tag_with_ruble` by [@quincylvania](https://github.com/quincylvania) ([#150](https://github.com/waysidemapping/pinhead/issues/150), [#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/campsite_with_yen_yuan.svg" width="15px"/> Add `campsite_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/campsite_with_rupee.svg" width="15px"/> Add `campsite_with_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/campsite_with_ruble.svg" width="15px"/> Add `campsite_with_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/tipi_campsite_with_yen_yuan.svg" width="15px"/> Add `tipi_campsite_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/tipi_campsite_with_rupee.svg" width="15px"/> Add `tipi_campsite_with_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/tipi_campsite_with_ruble.svg" width="15px"/> Add `tipi_campsite_with_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/bicycle_and_yen_yuan.svg" width="15px"/> Add `bicycle_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/bicycle_and_rupee.svg" width="15px"/> Add `bicycle_and_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/bicycle_and_ruble.svg" width="15px"/> Add `bicycle_and_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/cargobike_and_yen_yuan.svg" width="15px"/> Add `cargobike_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/cargobike_and_rupee.svg" width="15px"/> Add `cargobike_and_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/cargobike_and_ruble.svg" width="15px"/> Add `cargobike_and_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/car_with_yen_yuan.svg" width="15px"/> Add `car_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/car_with_rupee.svg" width="15px"/> Add `car_with_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/car_with_ruble.svg" width="15px"/> Add `car_with_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/person_using_terminal_kiosk_with_euro.svg" width="15px"/> Add `person_using_terminal_kiosk_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/person_using_terminal_kiosk_with_yen_yuan.svg" width="15px"/> Add `person_using_terminal_kiosk_with_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/person_using_terminal_kiosk_with_rupee.svg" width="15px"/> Add `person_using_terminal_kiosk_with_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/person_using_terminal_kiosk_with_ruble.svg" width="15px"/> Add `person_using_terminal_kiosk_with_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/person_using_terminal_kiosk_with_pound.svg" width="15px"/> Add `person_using_terminal_kiosk_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/milk_carton_and_apple.svg" width="15px"/> Add `milk_carton_and_apple` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_dollar.svg" width="15px"/> Add `milk_carton_and_apple_and_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_pound.svg" width="15px"/> Add `milk_carton_and_apple_and_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_yen_yuan.svg" width="15px"/> Add `milk_carton_and_apple_and_yen_yuan` by [@quincylvania](https://github.com/quincylvania) ([#77](https://github.com/waysidemapping/pinhead/issues/77))
- <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_rupee.svg" width="15px"/> Add `milk_carton_and_apple_and_rupee` by [@quincylvania](https://github.com/quincylvania) ([#79](https://github.com/waysidemapping/pinhead/issues/79))
- <img src="https://pinhead.ink/v19/milk_carton_and_apple_and_ruble.svg" width="15px"/> Add `milk_carton_and_apple_and_ruble` by [@quincylvania](https://github.com/quincylvania) ([#80](https://github.com/waysidemapping/pinhead/issues/80))
- <img src="https://pinhead.ink/v19/noodle_bowl_with_steam.svg" width="15px"/> Add `noodle_bowl_with_steam` by [@westnordost](https://github.com/westnordost) ([#146](https://github.com/waysidemapping/pinhead/issues/146))
- <img src="https://pinhead.ink/v19/apple_core.svg" width="15px"/> Add `apple_core` by [@quincylvania](https://github.com/quincylvania)

## [15.18.0] - 2026-03-19

_Pinhead v18_

This release contains new icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

- <img src="https://pinhead.ink/v18/double_diamond_tall.svg" width="15px"/> Add `double_diamond_tall` by [@dschep](https://github.com/dschep) ([#144](https://github.com/waysidemapping/pinhead/issues/144))
- <img src="https://pinhead.ink/v18/turntable.svg" width="15px"/> Add `turntable` by [@ooosssay](https://github.com/ooosssay) ([##143](https://github.com/waysidemapping/pinhead/issues/#143))
- <img src="https://pinhead.ink/v18/exclamation_point.svg" width="15px"/> Add `exclamation_point` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/wheelie_bin.svg" width="15px"/> Add `wheelie_bin` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wheelie_bin_and_bag_of_trash.svg" width="15px"/> Add `wheelie_bin_and_bag_of_trash` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wheelie_bin_and_drink_bottle_and_can.svg" width="15px"/> Add `wheelie_bin_and_drink_bottle_and_can` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wheelie_bin_and_leaf.svg" width="15px"/> Add `wheelie_bin_and_leaf` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wheelie_bin_and_apple_core.svg" width="15px"/> Add `wheelie_bin_and_apple_core` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/calendar_with_wheelie_bin.svg" width="15px"/> Add `calendar_with_wheelie_bin` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/trash_truck.svg" width="15px"/> Add `trash_truck` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/drink_bottle_and_milk_carton_and_can.svg" width="15px"/> Add `drink_bottle_and_milk_carton_and_can` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/person_reaching_into_bins.svg" width="15px"/> Add `person_reaching_into_bins` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/bag_of_trash_with_stink.svg" width="15px"/> Add `bag_of_trash_with_stink` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/bag_of_trash.svg" width="15px"/> Add `bag_of_trash` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/calendar.svg" width="15px"/> Add `calendar` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/parachute.svg" width="15px"/> Add `parachute` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/milk_carton_and_apple_and_euro.svg" width="15px"/> Add `milk_carton_and_apple_and_euro` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/triangle_up_with_skull.svg" width="15px"/> Add `triangle_up_with_skull` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/megaphone.svg" width="15px"/> Add `megaphone` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/crowd_of_people.svg" width="15px"/> Add `crowd_of_people` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/dove_and_laurel.svg" width="15px"/> Add `dove_and_laurel` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/dove.svg" width="15px"/> Add `dove` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/speech_bubbles.svg" width="15px"/> Add `speech_bubbles` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141), [#50](https://github.com/waysidemapping/pinhead/issues/50))
- <img src="https://pinhead.ink/v18/speech_bubble.svg" width="15px"/> Add `speech_bubble` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141), [#50](https://github.com/waysidemapping/pinhead/issues/50))
- <img src="https://pinhead.ink/v18/hairy_caterpillar_and_exclamation_point.svg" width="15px"/> Add `hairy_caterpillar_and_exclamation_point` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) with edits ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/hairy_caterpillar.svg" width="15px"/> Add `hairy_caterpillar` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/big_top_tent_with_pennant.svg" width="15px"/> Add `big_top_tent_with_pennant` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/canister_vacuum_cleaner.svg" width="15px"/> Add `canister_vacuum_cleaner` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/id_card.svg" width="15px"/> Add `id_card` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/key_with_house_keychain.svg" width="15px"/> Add `key_with_house_keychain` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/horse_head_wearing_bridle.svg" width="15px"/> Add `horse_head_wearing_bridle` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/gull_and_exclamation_point.svg" width="15px"/> Add `gull_and_exclamation_point` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) with edits ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/gull.svg" width="15px"/> Add `gull` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/handshake.svg" width="15px"/> Add `handshake` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/thumbs_up_hand_with_sleeve.svg" width="15px"/> Add `thumbs_up_hand_with_sleeve` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/passport_with_graticule_globe.svg" width="15px"/> Add `passport_with_graticule_globe` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/a_frame_signboard.svg" width="15px"/> Add `a_frame_signboard` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/bishops_miter_with_latin_cross_beside_crozier_head.svg" width="15px"/> Add `bishops_miter_with_latin_cross_beside_crozier_head` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/ring_linked_to_ring_with_jewel.svg" width="15px"/> Add `ring_linked_to_ring_with_jewel` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/greenhouse.svg" width="15px"/> Add `greenhouse` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/syringe.svg" width="15px"/> Add `syringe` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/person_walking_with_hiking_pole.svg" width="15px"/> Add `person_walking_with_hiking_pole` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/person_shoveling_dirt.svg" width="15px"/> Add `person_shoveling_dirt` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wolf_head_and_exclamation_point.svg" width="15px"/> Add `wolf_head_and_exclamation_point` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) with edits ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/wolf_head.svg" width="15px"/> Add `wolf_head` by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/magnifying_glass.svg" width="15px"/> Add `magnifying_glass` from [OpenGemeenten](https://github.com/OpenGemeenten/Iconenset) imported by [@quincylvania](https://github.com/quincylvania) ([#141](https://github.com/waysidemapping/pinhead/issues/141))
- <img src="https://pinhead.ink/v18/droplet_from_pipes.svg" width="15px"/> Add `droplet_from_pipes` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/bicycle_in_rectangle_outline.svg" width="15px"/> Add `bicycle_in_rectangle_outline` by [@quincylvania](https://github.com/quincylvania) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/motorboat_in_parking_structure.svg" width="15px"/> Add `motorboat_in_parking_structure` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/motorboat_on_parking_line.svg" width="15px"/> Add `motorboat_on_parking_line` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_using_terminal_kiosk.svg" width="15px"/> Add `person_using_terminal_kiosk` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_using_terminal_kiosk_with_dollar.svg" width="15px"/> Add `person_using_terminal_kiosk_with_dollar` from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania) with edits
- <img src="https://pinhead.ink/v18/activity_panel.svg" width="15px"/> Add `activity_panel` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/basket_swing.svg" width="15px"/> Add `basket_swing` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/swing.svg" width="15px"/> Add `swing` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/climbing_wall.svg" width="15px"/> Add `climbing_wall` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/play_shelter.svg" width="15px"/> Add `play_shelter` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_climbing_on_climbing_frame.svg" width="15px"/> Add `person_climbing_on_climbing_frame` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_jumping_in_puddle_with_splashes.svg" width="15px"/> Add `person_jumping_in_puddle_with_splashes` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_jumping_on_bouncy_cushion.svg" width="15px"/> Add `person_jumping_on_bouncy_cushion` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_jumping_on_trampoline.svg" width="15px"/> Add `person_jumping_on_trampoline` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v18/person_with_ponytail_riding_zip_line.svg" width="15px"/> Add `person_with_ponytail_riding_zip_line` by [@marensiegel](https://github.com/marensiegel) from [Temaki](https://github.com/rapideditor/temaki) imported by [@quincylvania](https://github.com/quincylvania)

## [15.17.0] - 2026-03-17

_Pinhead v17_

This release contains new, renamed, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v16/plane.svg" width="15px"/> `plane` -> <img src="https://pinhead.ink/v17/plane_up.svg" width="15px"/> `plane_up` ([#128](https://github.com/waysidemapping/pinhead/issues/128))

### Renamed icons

- <img src="https://pinhead.ink/v17/new_hampshire.svg" width="15px"/> `new_hampsire` -> `new_hampshire`
- <img src="https://pinhead.ink/v17/new_hampshire_with_capital_star.svg" width="15px"/> `new_hampsire_with_capital_star` -> `new_hampshire_with_capital_star`

### Redesigned icons

- <img src="https://pinhead.ink/v16/barbell.svg" width="15px"/> -> <img src="https://pinhead.ink/v17/barbell.svg" width="15px"/> `barbell` ([#124](https://github.com/waysidemapping/pinhead/issues/124))
- <img src="https://pinhead.ink/v16/paperclip.svg" width="15px"/> -> <img src="https://pinhead.ink/v17/paperclip.svg" width="15px"/> `paperclip` ([#126](https://github.com/waysidemapping/pinhead/issues/126))
- <img src="https://pinhead.ink/v16/banknote_in_slot.svg" width="15px"/> -> <img src="https://pinhead.ink/v17/banknote_in_slot.svg" width="15px"/> `banknote_in_slot` ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v16/envelope_in_slot.svg" width="15px"/> -> <img src="https://pinhead.ink/v17/envelope_in_slot.svg" width="15px"/> `envelope_in_slot` ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v16/ticket_in_slot.svg" width="15px"/> -> <img src="https://pinhead.ink/v17/ticket_in_slot.svg" width="15px"/> `ticket_in_slot` ([#139](https://github.com/waysidemapping/pinhead/issues/139))

### Added icons

- <img src="https://pinhead.ink/v17/bee.svg" width="15px"/> Add `bee` by [@westnordost](https://github.com/westnordost) ([#125](https://github.com/waysidemapping/pinhead/issues/125), [#121](https://github.com/waysidemapping/pinhead/issues/121))
- <img src="https://pinhead.ink/v17/bee_skep.svg" width="15px"/> Add `bee_skep` by [@westnordost](https://github.com/westnordost) ([#125](https://github.com/waysidemapping/pinhead/issues/125))
- <img src="https://pinhead.ink/v17/honeycomb.svg" width="15px"/> Add `honeycomb` by [@westnordost](https://github.com/westnordost) ([#125](https://github.com/waysidemapping/pinhead/issues/125))
- <img src="https://pinhead.ink/v17/bohr_atomic_model.svg" width="15px"/> Add `bohr_atomic_model` by [@westnordost](https://github.com/westnordost) ([#136](https://github.com/waysidemapping/pinhead/issues/136))
- <img src="https://pinhead.ink/v17/elephant.svg" width="15px"/> Add `elephant` from [source](https://upload.wikimedia.org/wikipedia/commons/0/02/MX_road_sign_SIT-56.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/rooster_fighting.svg" width="15px"/> Add `rooster_fighting` from [source](https://upload.wikimedia.org/wikipedia/commons/9/98/MX_road_sign_SIT-42.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/baseball_bat_and_baseball.svg" width="15px"/> Add `baseball_bat_and_baseball` from [source](https://upload.wikimedia.org/wikipedia/commons/f/f5/MX_road_sign_SIT-21.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/boxing_glove_up.svg" width="15px"/> Add `boxing_glove_up` from [source](https://upload.wikimedia.org/wikipedia/commons/5/5c/MX_road_sign_SIT-64.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/jai_alai_cesta_and_ball.svg" width="15px"/> Add `jai_alai_cesta_and_ball` from [source](https://upload.wikimedia.org/wikipedia/commons/a/a3/MX_road_sign_SIT-35.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_dancing_with_person_wearing_dress.svg" width="15px"/> Add `person_dancing_with_person_wearing_dress` from [source](https://upload.wikimedia.org/wikipedia/commons/d/da/MX_road_sign_SIT-58.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/people_wearing_traditional_festive_latin_clothes.svg" width="15px"/> Add `people_wearing_traditional_festive_latin_clothes` from [source](https://upload.wikimedia.org/wikipedia/commons/b/bc/MX_road_sign_SIT-27.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_wearing_martial_arts_belt_front_kicking.svg" width="15px"/> Add `person_wearing_martial_arts_belt_front_kicking` from [source](https://upload.wikimedia.org/wikipedia/commons/c/c6/MX_road_sign_SIT-62.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_holding_barbell.svg" width="15px"/> Add `person_holding_barbell` from [source](https://upload.wikimedia.org/wikipedia/commons/4/4d/MX_road_sign_SIT-70.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_wearing_racing_helmet_driving_go_kart.svg" width="15px"/> Add `person_wearing_racing_helmet_driving_go_kart` from [source](https://upload.wikimedia.org/wikipedia/commons/d/dc/MX_road_sign_SIT-31.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_leaping_over_hurdle.svg" width="15px"/> Add `person_leaping_over_hurdle` from [source](https://upload.wikimedia.org/wikipedia/commons/d/da/MX_road_sign_SIT-63.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_standing.svg" width="15px"/> Add `person_standing` from [source](https://upload.wikimedia.org/wikipedia/commons/4/4d/MX_road_sign_SIT-70.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/person_wearing_cowboy_hat_holding_coiled_rope.svg" width="15px"/> Add `person_wearing_cowboy_hat_holding_coiled_rope` from [source](https://upload.wikimedia.org/wikipedia/commons/f/f1/MX_road_sign_SIT-38.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/ice_skate.svg" width="15px"/> Add `ice_skate` from [source](https://upload.wikimedia.org/wikipedia/commons/e/e6/MX_road_sign_SIT-69.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/inline_skate.svg" width="15px"/> Add `inline_skate` from [source](https://upload.wikimedia.org/wikipedia/commons/6/63/MX_road_sign_SIT-68.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/chess_knight.svg" width="15px"/> Add `chess_knight` from [source](https://upload.wikimedia.org/wikipedia/commons/7/74/MX_road_sign_SIT-36.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/lucha_libre_mask.svg" width="15px"/> Add `lucha_libre_mask` from [source](https://upload.wikimedia.org/wikipedia/commons/c/c1/MX_road_sign_SIT-61.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/soccer_ball.svg" width="15px"/> Add `soccer_ball` from [source](https://upload.wikimedia.org/wikipedia/commons/d/d9/MX_road_sign_SIT-28.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#127](https://github.com/waysidemapping/pinhead/issues/127))
- <img src="https://pinhead.ink/v17/slot.svg" width="15px"/> Add `slot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v17/vertical_slot.svg" width="15px"/> Add `vertical_slot` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v17/arrow_down_from_banknote_in_slot.svg" width="15px"/> Add `arrow_down_from_banknote_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_up_to_banknote_in_slot.svg" width="15px"/> Add `arrow_up_to_banknote_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_down_from_envelope_in_slot.svg" width="15px"/> Add `arrow_down_from_envelope_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_up_to_envelope_in_slot.svg" width="15px"/> Add `arrow_up_to_envelope_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/payment_card.svg" width="15px"/> Add `payment_card` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/payment_card_in_slot.svg" width="15px"/> Add `payment_card_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_down_from_payment_card_in_slot.svg" width="15px"/> Add `arrow_down_from_payment_card_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_up_to_payment_card_in_slot.svg" width="15px"/> Add `arrow_up_to_payment_card_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_down_from_ticket_in_slot.svg" width="15px"/> Add `arrow_down_from_ticket_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/arrow_up_to_ticket_in_slot.svg" width="15px"/> Add `arrow_up_to_ticket_in_slot` by [@ooosssay](https://github.com/ooosssay) ([#139](https://github.com/waysidemapping/pinhead/issues/139))
- <img src="https://pinhead.ink/v17/plane_top_right.svg" width="15px"/> Add `plane_top_right` by [@quincylvania](https://github.com/quincylvania) ([#128](https://github.com/waysidemapping/pinhead/issues/128))
- <img src="https://pinhead.ink/v17/plane_right.svg" width="15px"/> Add `plane_right` by [@quincylvania](https://github.com/quincylvania) ([#128](https://github.com/waysidemapping/pinhead/issues/128))
- <img src="https://pinhead.ink/v17/stone_arrowhead_up.svg" width="15px"/> Add `stone_arrowhead_up` by [@quincylvania](https://github.com/quincylvania) ([#115](https://github.com/waysidemapping/pinhead/issues/115))
- <img src="https://pinhead.ink/v17/stone_arrowhead_top_right.svg" width="15px"/> Add `stone_arrowhead_top_right` by [@quincylvania](https://github.com/quincylvania) ([#115](https://github.com/waysidemapping/pinhead/issues/115))
- <img src="https://pinhead.ink/v17/stone_arrowhead_right.svg" width="15px"/> Add `stone_arrowhead_right` by [@quincylvania](https://github.com/quincylvania) ([#115](https://github.com/waysidemapping/pinhead/issues/115))
- <img src="https://pinhead.ink/v17/stone_arrowhead_down.svg" width="15px"/> Add `stone_arrowhead_down` by [@quincylvania](https://github.com/quincylvania) ([#115](https://github.com/waysidemapping/pinhead/issues/115))
- <img src="https://pinhead.ink/v17/hash.svg" width="15px"/> Add `hash` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v17/bicycle_and_dollar.svg" width="15px"/> Add `bicycle_and_dollar` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/bicycle_and_euro.svg" width="15px"/> Add `bicycle_and_euro` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/bicycle_and_pound.svg" width="15px"/> Add `bicycle_and_pound` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/cargobike_and_dollar.svg" width="15px"/> Add `cargobike_and_dollar` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/cargobike_and_euro.svg" width="15px"/> Add `cargobike_and_euro` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/cargobike_and_pound.svg" width="15px"/> Add `cargobike_and_pound` by [@quincylvania](https://github.com/quincylvania) ([#91](https://github.com/waysidemapping/pinhead/issues/91))
- <img src="https://pinhead.ink/v17/campsite_and_droplet.svg" width="15px"/> Add `campsite_and_droplet` by [@quincylvania](https://github.com/quincylvania) ([#134](https://github.com/waysidemapping/pinhead/issues/134))
- <img src="https://pinhead.ink/v17/tipi_campsite_and_droplet.svg" width="15px"/> Add `tipi_campsite_and_droplet` by [@quincylvania](https://github.com/quincylvania) ([#134](https://github.com/waysidemapping/pinhead/issues/134))
- <img src="https://pinhead.ink/v17/campsite_and_wifi.svg" width="15px"/> Add `campsite_and_wifi` by [@quincylvania](https://github.com/quincylvania)

## [15.16.0] - 2026-03-15

_Pinhead v16_

This release contains new, merged, and redesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Merged icons

- <img src="https://pinhead.ink/v15/jp_school.svg" width="15px"/> `jp_school` -> <img src="https://pinhead.ink/v16/jp_college.svg" width="15px"/> `jp_college`

### Redesigned icons

- <img src="https://pinhead.ink/v15/delicate_arch.svg" width="15px"/> -> <img src="https://pinhead.ink/v16/delicate_arch.svg" width="15px"/> `delicate_arch`
- <img src="https://pinhead.ink/v15/crystal_ball_on_sphere_stand.svg" width="15px"/> -> <img src="https://pinhead.ink/v16/crystal_ball_on_sphere_stand.svg" width="15px"/> `crystal_ball_on_sphere_stand` ([#116](https://github.com/waysidemapping/pinhead/issues/116))

### Added icons

- <img src="https://pinhead.ink/v16/steel_square_and_drafting_compass.svg" width="15px"/> Add `steel_square_and_drafting_compass` by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/madison_cross.svg" width="15px"/> Add `madison_cross` by [@quincylvania](https://github.com/quincylvania) ([#112](https://github.com/waysidemapping/pinhead/issues/112))
- <img src="https://pinhead.ink/v16/keystone.svg" width="15px"/> Add `keystone` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v16/ethernet_port.svg" width="15px"/> Add `ethernet_port` by [@quincylvania](https://github.com/quincylvania) ([#110](https://github.com/waysidemapping/pinhead/issues/110))
- <img src="https://pinhead.ink/v16/ethernet_port_in_square.svg" width="15px"/> Add `ethernet_port_in_square` by [@quincylvania](https://github.com/quincylvania) ([#110](https://github.com/waysidemapping/pinhead/issues/110))
- <img src="https://pinhead.ink/v16/cup_and_saucer_and_wifi.svg" width="15px"/> Add `cup_and_saucer_and_wifi` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v16/pixel_ape_face_with_eye_patch.svg" width="15px"/> Add `pixel_ape_face_with_eye_patch` by [@quincylvania](https://github.com/quincylvania)

Add icons sourced from Secretaría de Infraestructura, Comunicaciones y Transportes (SICT) & Secretaría de Desarrollo Agrario, Territorial y Urbano (SEDATU):

- <img src="https://pinhead.ink/v16/typha_and_duck_in_water.svg" width="15px"/> Add `typha_and_duck_in_water` from [source](https://upload.wikimedia.org/wikipedia/commons/c/c7/MX_road_sign_SIT-6.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/dome_with_crescent_moon_and_star_and_planet.svg" width="15px"/> Add `dome_with_crescent_moon_and_star_and_planet` from [source](https://upload.wikimedia.org/wikipedia/commons/6/6d/MX_road_sign_SIT-12.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/mesoamerican_pyramid.svg" width="15px"/> Add `mesoamerican_pyramid` from [source](https://upload.wikimedia.org/wikipedia/commons/4/4c/MX_road_sign_SIT-10.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/badminton_racket_and_shuttlecock.svg" width="15px"/> Add `badminton_racket_and_shuttlecock` from [source](https://upload.wikimedia.org/wikipedia/commons/0/0b/MX_road_sign_SIT-18.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/person_behind_desk.svg" width="15px"/> Add `person_behind_desk` from [source](https://upload.wikimedia.org/wikipedia/commons/7/7b/MX_road_sign_SIT-13.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/person_in_water_with_steam.svg" width="15px"/> Add `person_in_water_with_steam` from [source](https://upload.wikimedia.org/wikipedia/commons/4/48/MX_road_sign_SIT-14.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/person_wearing_racing_helmet_driving_racecar.svg" width="15px"/> Add `person_wearing_racing_helmet_driving_racecar` from [source](https://upload.wikimedia.org/wikipedia/commons/b/b2/MX_road_sign_SIT-17.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))
- <img src="https://pinhead.ink/v16/person_walking_bicycle.svg" width="15px"/> Add `person_walking_bicycle` from [source](https://upload.wikimedia.org/wikipedia/commons/5/57/MX_road_sign_SR-43A.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116), [#88](https://github.com/waysidemapping/pinhead/issues/88))
- <img src="https://pinhead.ink/v16/traditional_storage_jars.svg" width="15px"/> Add `traditional_storage_jars` from [source](https://upload.wikimedia.org/wikipedia/commons/5/58/MX_road_sign_SIT-2.svg) imported by [@ooosssay](https://github.com/ooosssay) ([#116](https://github.com/waysidemapping/pinhead/issues/116))

Add icons for US boundaries:

- <img src="https://pinhead.ink/v16/contiguous_united_states.svg" width="15px"/> Add `contiguous_united_states` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/contiguous_united_states_with_capital_star.svg" width="15px"/> Add `contiguous_united_states_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/alabama.svg" width="15px"/> Add `alabama` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/alabama_with_capital_star.svg" width="15px"/> Add `alabama_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/alaska.svg" width="15px"/> Add `alaska` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/arizona.svg" width="15px"/> Add `arizona` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/arizona_with_capital_star.svg" width="15px"/> Add `arizona_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/arkansas.svg" width="15px"/> Add `arkansas` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/arkansas_with_capital_star.svg" width="15px"/> Add `arkansas_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/california.svg" width="15px"/> Add `california` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/california_with_capital_star.svg" width="15px"/> Add `california_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/colorado.svg" width="15px"/> Add `colorado` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/colorado_with_capital_star.svg" width="15px"/> Add `colorado_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/connecticut.svg" width="15px"/> Add `connecticut` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/connecticut_with_capital_star.svg" width="15px"/> Add `connecticut_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/delaware.svg" width="15px"/> Add `delaware` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/delaware_with_capital_star.svg" width="15px"/> Add `delaware_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/district_of_columbia.svg" width="15px"/> Add `district_of_columbia` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/district_of_columbia_with_capital_star.svg" width="15px"/> Add `district_of_columbia_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/florida.svg" width="15px"/> Add `florida` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/georgia_us.svg" width="15px"/> Add `georgia_us` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/georgia_us_with_capital_star.svg" width="15px"/> Add `georgia_us_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/hawaii.svg" width="15px"/> Add `hawaii` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/idaho.svg" width="15px"/> Add `idaho` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/idaho_with_capital_star.svg" width="15px"/> Add `idaho_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/illinois.svg" width="15px"/> Add `illinois` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/illinois_with_capital_star.svg" width="15px"/> Add `illinois_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/indiana.svg" width="15px"/> Add `indiana` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/indiana_with_capital_star.svg" width="15px"/> Add `indiana_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/iowa.svg" width="15px"/> Add `iowa` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/iowa_with_capital_star.svg" width="15px"/> Add `iowa_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/kansas.svg" width="15px"/> Add `kansas` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/kansas_with_capital_star.svg" width="15px"/> Add `kansas_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/kentucky.svg" width="15px"/> Add `kentucky` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/kentucky_with_capital_star.svg" width="15px"/> Add `kentucky_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/louisiana.svg" width="15px"/> Add `louisiana` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/louisiana_with_capital_star.svg" width="15px"/> Add `louisiana_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/maine.svg" width="15px"/> Add `maine` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/maine_with_capital_star.svg" width="15px"/> Add `maine_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/maryland.svg" width="15px"/> Add `maryland` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/massachusetts.svg" width="15px"/> Add `massachusetts` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/massachusetts_with_capital_star.svg" width="15px"/> Add `massachusetts_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/michigan.svg" width="15px"/> Add `michigan` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/michigan_with_capital_star.svg" width="15px"/> Add `michigan_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/michigan_lower_peninsula.svg" width="15px"/> Add `michigan_lower_peninsula` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/michigan_upper_peninsula.svg" width="15px"/> Add `michigan_upper_peninsula` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/minnesota.svg" width="15px"/> Add `minnesota` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/minnesota_with_capital_star.svg" width="15px"/> Add `minnesota_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/mississippi.svg" width="15px"/> Add `mississippi` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/mississippi_with_capital_star.svg" width="15px"/> Add `mississippi_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/missouri.svg" width="15px"/> Add `missouri` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/missouri_with_capital_star.svg" width="15px"/> Add `missouri_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/montana.svg" width="15px"/> Add `montana` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/montana_with_capital_star.svg" width="15px"/> Add `montana_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/nebraska.svg" width="15px"/> Add `nebraska` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/nebraska_with_capital_star.svg" width="15px"/> Add `nebraska_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/nevada.svg" width="15px"/> Add `nevada` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/nevada_with_capital_star.svg" width="15px"/> Add `nevada_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_hampsire.svg" width="15px"/> Add `new_hampsire` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_hampsire_with_capital_star.svg" width="15px"/> Add `new_hampsire_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_jersey.svg" width="15px"/> Add `new_jersey` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_jersey_with_capital_star.svg" width="15px"/> Add `new_jersey_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_mexico.svg" width="15px"/> Add `new_mexico` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_mexico_with_capital_star.svg" width="15px"/> Add `new_mexico_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_york.svg" width="15px"/> Add `new_york` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/new_york_with_capital_star.svg" width="15px"/> Add `new_york_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/north_dakota.svg" width="15px"/> Add `north_dakota` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/north_dakota_with_capital_star.svg" width="15px"/> Add `north_dakota_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/north_carolina.svg" width="15px"/> Add `north_carolina` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/north_carolina_with_capital_star.svg" width="15px"/> Add `north_carolina_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/ohio.svg" width="15px"/> Add `ohio` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/ohio_with_capital_star.svg" width="15px"/> Add `ohio_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/oklahoma.svg" width="15px"/> Add `oklahoma` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/oklahoma_with_capital_star.svg" width="15px"/> Add `oklahoma_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/oregon.svg" width="15px"/> Add `oregon` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/oregon_with_capital_star.svg" width="15px"/> Add `oregon_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/pennsylvania.svg" width="15px"/> Add `pennsylvania` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/pennsylvania_with_capital_star.svg" width="15px"/> Add `pennsylvania_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/rhode_island.svg" width="15px"/> Add `rhode_island` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/rhode_island_with_capital_star.svg" width="15px"/> Add `rhode_island_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/south_dakota.svg" width="15px"/> Add `south_dakota` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/south_dakota_with_capital_star.svg" width="15px"/> Add `south_dakota_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/south_carolina.svg" width="15px"/> Add `south_carolina` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/south_carolina_with_capital_star.svg" width="15px"/> Add `south_carolina_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/tennessee.svg" width="15px"/> Add `tennessee` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/tennessee_with_capital_star.svg" width="15px"/> Add `tennessee_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/texas.svg" width="15px"/> Add `texas` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/texas_with_capital_star.svg" width="15px"/> Add `texas_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/utah.svg" width="15px"/> Add `utah` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/utah_with_capital_star.svg" width="15px"/> Add `utah_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/vermont.svg" width="15px"/> Add `vermont` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/vermont_with_capital_star.svg" width="15px"/> Add `vermont_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/virginia.svg" width="15px"/> Add `virginia` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/virginia_with_capital_star.svg" width="15px"/> Add `virginia_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/washington.svg" width="15px"/> Add `washington` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/washington_with_capital_star.svg" width="15px"/> Add `washington_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/west_virginia.svg" width="15px"/> Add `west_virginia` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/west_virginia_with_capital_star.svg" width="15px"/> Add `west_virginia_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/wisconsin.svg" width="15px"/> Add `wisconsin` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/wisconsin_with_capital_star.svg" width="15px"/> Add `wisconsin_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/wyoming.svg" width="15px"/> Add `wyoming` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))
- <img src="https://pinhead.ink/v16/wyoming_with_capital_star.svg" width="15px"/> Add `wyoming_with_capital_star` by [@quincylvania](https://github.com/quincylvania) ([#114](https://github.com/waysidemapping/pinhead/issues/114))

## [15.15.0] - 2026-03-11

_Pinhead v15_

⚠️ This major release contains new, resdesigned, and renamed icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Distribution changes

The Pinhead version number now corresponds to the minor version (the middle number) instead of the major version (the first number) of the release version number.

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v14/water_glass_under_faucet.svg" width="15px"/> `water_glass_under_faucet` -> <img src="https://pinhead.ink/v15/water_tap_with_drinking_glass.svg" width="15px"/> `water_tap_with_drinking_glass`
- <img src="https://pinhead.ink/v14/water_faucet_with_droplet.svg" width="15px"/> `water_faucet_with_droplet` -> <img src="https://pinhead.ink/v15/water_tap_with_handle_and_droplet.svg" width="15px"/> `water_tap_with_handle_and_droplet`
- <img src="https://pinhead.ink/v14/water_tap.svg" width="15px"/> `water_tap` -> <img src="https://pinhead.ink/v15/water_standpipe_with_handle.svg" width="15px"/> `water_standpipe_with_handle`
- <img src="https://pinhead.ink/v14/water_glass_under_water_tap.svg" width="15px"/> `water_glass_under_water_tap` -> <img src="https://pinhead.ink/v15/water_standpipe_with_handle_and_drinking_glass.svg" width="15px"/> `water_standpipe_with_handle_and_drinking_glass`
- <img src="https://pinhead.ink/v14/water_tap_with_pump_handle.svg" width="15px"/> `water_tap_with_pump_handle` -> <img src="https://pinhead.ink/v15/water_standpipe_with_pump_handle.svg" width="15px"/> `water_standpipe_with_pump_handle`
- <img src="https://pinhead.ink/v14/water_tap_with_motor.svg" width="15px"/> `water_tap_with_motor` -> <img src="https://pinhead.ink/v15/water_standpipe_with_motor_and_handle.svg" width="15px"/> `water_standpipe_with_motor_and_handle`
- <img src="https://pinhead.ink/v14/water_pipe_with_motor.svg" width="15px"/> `water_pipe_with_motor` -> <img src="https://pinhead.ink/v15/water_pipe_return_bend_with_motor_and_handle.svg" width="15px"/> `water_pipe_return_bend_with_motor_and_handle`

### Added icons

Add icons by new contributor [@ooosssay](https://github.com/ooosssay). Thanks, @ooosssay!

- <img src="https://pinhead.ink/v15/crystal_ball_on_sphere_stand.svg" width="15px"/> Add `crystal_ball_on_sphere_stand` by [@ooosssay](https://github.com/ooosssay) ([#106](https://github.com/waysidemapping/pinhead/issues/106))
- <img src="https://pinhead.ink/v15/piano_keys.svg" width="15px"/> Add `piano_keys` by [@ooosssay](https://github.com/ooosssay) ([#103](https://github.com/waysidemapping/pinhead/issues/103))
- <img src="https://pinhead.ink/v15/hand_dropping_circles.svg" width="15px"/> Add `hand_dropping_circles` by [@ooosssay](https://github.com/ooosssay) ([#103](https://github.com/waysidemapping/pinhead/issues/103))
- <img src="https://pinhead.ink/v15/hand_dropping_circles_into_container.svg" width="15px"/> Add `hand_dropping_circles_into_container` by [@ooosssay](https://github.com/ooosssay) ([#103](https://github.com/waysidemapping/pinhead/issues/103))

Add assorted icons:

- <img src="https://pinhead.ink/v15/mounted_slotted_dispenser.svg" width="15px"/> Add `mounted_slotted_dispenser` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/mounted_slotted_dispenser_with_poo_pile.svg" width="15px"/> Add `mounted_slotted_dispenser_with_poo_pile` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/antler.svg" width="15px"/> Add `antler` by [@quincylvania](https://github.com/quincylvania) ([#86](https://github.com/waysidemapping/pinhead/issues/86))
- <img src="https://pinhead.ink/v15/bone.svg" width="15px"/> Add `bone` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/jack_o_lantern.svg" width="15px"/> Add `jack_o_lantern` by [@quincylvania](https://github.com/quincylvania) ([#83](https://github.com/waysidemapping/pinhead/issues/83))
- <img src="https://pinhead.ink/v15/compact_box_truck_with_box_peak.svg" width="15px"/> Add `compact_box_truck_with_box_peak` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/sub_sandwich_with_steam.svg" width="15px"/> Add `sub_sandwich_with_steam` by [@quincylvania](https://github.com/quincylvania) ([#101](https://github.com/waysidemapping/pinhead/issues/101))
- <img src="https://pinhead.ink/v15/vinyl_record.svg" width="15px"/> Add `vinyl_record` by [@quincylvania](https://github.com/quincylvania) ([#70](https://github.com/waysidemapping/pinhead/issues/70))
- <img src="https://pinhead.ink/v15/winding_way_narrow.svg" width="15px"/> Add `winding_way_narrow` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/winding_way.svg" width="15px"/> Add `winding_way` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/winding_way_wide.svg" width="15px"/> Add `winding_way_wide` by [@quincylvania](https://github.com/quincylvania)

Add pixel icons:

- <img src="https://pinhead.ink/v15/pixel_ape_face.svg" width="15px"/> Add `pixel_ape_face` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/pixel_three_inch_floppy_disk.svg" width="15px"/> Add `pixel_three_inch_floppy_disk` by [@quincylvania](https://github.com/quincylvania)

Add more water access icon variants:

- <img src="https://pinhead.ink/v15/water_tap.svg" width="15px"/> Add `water_tap` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_tap_with_droplet.svg" width="15px"/> Add `water_tap_with_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_tap_with_handle.svg" width="15px"/> Add `water_tap_with_handle` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_tap_with_handle_and_drinking_glass.svg" width="15px"/> Add `water_tap_with_handle_and_drinking_glass` by [@quincylvania](https://github.com/quincylvania) ([#52](https://github.com/waysidemapping/pinhead/issues/52))
- <img src="https://pinhead.ink/v15/water_standpipe_with_handle_and_droplet.svg" width="15px"/> Add `water_standpipe_with_handle_and_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_standpipe_with_pump_handle_and_droplet.svg" width="15px"/> Add `water_standpipe_with_pump_handle_and_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_standpipe_with_pump_handle_and_drinking_glass.svg" width="15px"/> Add `water_standpipe_with_pump_handle_and_drinking_glass` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_standpipe_with_motor_and_handle_and_droplet.svg" width="15px"/> Add `water_standpipe_with_motor_and_handle_and_droplet` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_standpipe_with_motor_and_handle_and_drinking_glass.svg" width="15px"/> Add `water_standpipe_with_motor_and_handle_and_drinking_glass` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v15/water_pipe_return_bend_with_handle.svg" width="15px"/> Add `water_pipe_return_bend_with_handle` by [@quincylvania](https://github.com/quincylvania)

Import assorted [Health Icons](https://github.com/resolvetosavelives/healthicons) ([CC0](https://healthicons.org/about#license)):

- <img src="https://pinhead.ink/v15/peace_sign.svg" width="15px"/> Add `peace_sign` ([#107](https://github.com/waysidemapping/pinhead/issues/107), [#75](https://github.com/waysidemapping/pinhead/issues/75))
- <img src="https://pinhead.ink/v15/biohazard_symbol.svg" width="15px"/> Add `biohazard_symbol` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/video_camera_symbol.svg" width="15px"/> Add `video_camera_symbol` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/mosquito.svg" width="15px"/> Add `mosquito` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/antibody.svg" width="15px"/> Add `antibody` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/anus.svg" width="15px"/> Add `anus` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/arm.svg" width="15px"/> Add `arm` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/bacteria.svg" width="15px"/> Add `bacteria` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/bladder.svg" width="15px"/> Add `bladder` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/blood_cells.svg" width="15px"/> Add `blood_cells` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/cell_nuclei.svg" width="15px"/> Add `cell_nuclei` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/dna.svg" width="15px"/> Add `dna` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/enzyme.svg" width="15px"/> Add `enzyme` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/female_groin.svg" width="15px"/> Add `female_groin` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/female_reproductive_system.svg" width="15px"/> Add `female_reproductive_system` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/fetus.svg" width="15px"/> Add `fetus` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/fetus_in_circle.svg" width="15px"/> Add `fetus_in_circle` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/fetus_in_circle_outline.svg" width="15px"/> Add `fetus_in_circle_outline` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/foot.svg" width="15px"/> Add `foot` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/gallbladder.svg" width="15px"/> Add `gallbladder` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/human_head.svg" width="15px"/> Add `human_head` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/heart_organ.svg" width="15px"/> Add `heart_organ` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/intestine.svg" width="15px"/> Add `intestine` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/joint.svg" width="15px"/> Add `joint` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/kidneys.svg" width="15px"/> Add `kidneys` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/leg.svg" width="15px"/> Add `leg` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/leg_with_varicose_veins.svg" width="15px"/> Add `leg_with_varicose_veins` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/lungs.svg" width="15px"/> Add `lungs` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/lungs_with_right_side_spots.svg" width="15px"/> Add `lungs_with_right_side_spots` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/male_genitalia.svg" width="15px"/> Add `male_genitalia` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/male_genitalia_with_urethra.svg" width="15px"/> Add `male_genitalia_with_urethra` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/male_genitalia_with_testicles.svg" width="15px"/> Add `male_genitalia_with_testicles` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/male_groin.svg" width="15px"/> Add `male_groin` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/nose_outline.svg" width="15px"/> Add `nose_outline` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/pancreas.svg" width="15px"/> Add `pancreas` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/prostate.svg" width="15px"/> Add `prostate` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/spleen.svg" width="15px"/> Add `spleen` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/stomach.svg" width="15px"/> Add `stomach` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/thyroid.svg" width="15px"/> Add `thyroid` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/tissue.svg" width="15px"/> Add `tissue` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/tumor.svg" width="15px"/> Add `tumor` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/person_with_open_arms.svg" width="15px"/> Add `person_with_open_arms` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/underweight_person.svg" width="15px"/> Add `underweight_person` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/overweight_person.svg" width="15px"/> Add `overweight_person` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/pregnant_person.svg" width="15px"/> Add `pregnant_person` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/person_vomiting.svg" width="15px"/> Add `person_vomiting` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/person_with_droplets.svg" width="15px"/> Add `person_with_droplets` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/person_walking_holding_railing.svg" width="15px"/> Add `person_walking_holding_railing` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/rememberance_ribbon.svg" width="15px"/> Add `rememberance_ribbon` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/face_mask.svg" width="15px"/> Add `face_mask` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/respirator.svg" width="15px"/> Add `respirator` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/diaper.svg" width="15px"/> Add `diaper` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/quadcopter_drone.svg" width="15px"/> Add `quadcopter_drone` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/sayana_press.svg" width="15px"/> Add `sayana_press` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/sperm.svg" width="15px"/> Add `sperm` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/condom.svg" width="15px"/> Add `condom` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/condom_and_venus.svg" width="15px"/> Add `condom_and_venus` ([#107](https://github.com/waysidemapping/pinhead/issues/107))
- <img src="https://pinhead.ink/v15/condom_and_mars.svg" width="15px"/> Add `condom_and_mars` ([#107](https://github.com/waysidemapping/pinhead/issues/107))

## [14.0.0] - 2026-03-08

⚠️ This major release contains new and resdesigned icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

Add dog icons:

- <img src="https://pinhead.ink/v14/dog.svg" width="15px"/> Add `dog` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/dog_wearing_collar_on_leash.svg" width="15px"/> Add `dog_wearing_collar_on_leash` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/dog_wearing_harness.svg" width="15px"/> Add `dog_wearing_harness` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/dog_wearing_harness_on_leash.svg" width="15px"/> Add `dog_wearing_harness_on_leash` by [@quincylvania](https://github.com/quincylvania)

Import icons from OpenStreetMap Carto and NPS:

- <img src="https://pinhead.ink/v14/cupcake_with_cherry.svg" width="15px"/> Add `cupcake_with_cherry`
- <img src="https://pinhead.ink/v14/milk_carton_and_cheese.svg" width="15px"/> Add `milk_carton_and_cheese`
- <img src="https://pinhead.ink/v14/rays_outward.svg" width="15px"/> Add `rays_outward`
- <img src="https://pinhead.ink/v14/dot_with_rays_right.svg" width="15px"/> Add `dot_with_rays_right`

Add train icon variants:

- <img src="https://pinhead.ink/v14/bullet_train.svg" width="15px"/> Add `bullet_train` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/diesel_train.svg" width="15px"/> Add `diesel_train` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/steam_train.svg" width="15px"/> Add `steam_train` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/steam_train_with_tires.svg" width="15px"/> Add `steam_train_with_tires` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/kids_train.svg" width="15px"/> Add `kids_train` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/kids_train_with_tires.svg" width="15px"/> Add `kids_train_with_tires` by [@quincylvania](https://github.com/quincylvania)

Add car icons:

- <img src="https://pinhead.ink/v14/car_beside_car.svg" width="15px"/> Add `car_beside_car` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/car_beside_car_under_car_beside_car.svg" width="15px"/> Add `car_beside_car_under_car_beside_car` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/car_under_toll_gantry.svg" width="15px"/> Add `car_under_toll_gantry` by [@quincylvania](https://github.com/quincylvania)

Add tag icons:

- <img src="https://pinhead.ink/v14/tag.svg" width="15px"/> Add `tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/car_and_tag.svg" width="15px"/> Add `car_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/sedan_and_tag.svg" width="15px"/> Add `sedan_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/station_wagon_and_tag.svg" width="15px"/> Add `station_wagon_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/pickup_truck_and_tag.svg" width="15px"/> Add `pickup_truck_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/bicycle_and_tag.svg" width="15px"/> Add `bicycle_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/motorcycle_and_tag.svg" width="15px"/> Add `motorcycle_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/cargobike_and_tag.svg" width="15px"/> Add `cargobike_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/motorboat_and_tag.svg" width="15px"/> Add `motorboat_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/vneck_tshirt_and_tag.svg" width="15px"/> Add `vneck_tshirt_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/giftwrapped_box_and_tag.svg" width="15px"/> Add `giftwrapped_box_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/file_box_and_tag.svg" width="15px"/> Add `file_box_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/shopping_bag_and_tag.svg" width="15px"/> Add `shopping_bag_and_tag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/shopping_bag_with_tag.svg" width="15px"/> Add `shopping_bag_with_tag` by [@quincylvania](https://github.com/quincylvania)

Add arrow icons:

- <img src="https://pinhead.ink/v14/arrow_left.svg" width="15px"/> Add `arrow_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_up.svg" width="15px"/> Add `arrow_up` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_down.svg" width="15px"/> Add `arrow_down` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_bottom_left.svg" width="15px"/> Add `arrow_bottom_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_bottom_right.svg" width="15px"/> Add `arrow_bottom_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_top_left.svg" width="15px"/> Add `arrow_top_left` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_top_right.svg" width="15px"/> Add `arrow_top_right` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_down_from_up_bracket.svg" width="15px"/> Add `arrow_down_from_up_bracket` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_right_from_left_bracket.svg" width="15px"/> Add `arrow_right_from_left_bracket` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v14/arrow_left_from_right_bracket.svg" width="15px"/> Add `arrow_left_from_right_bracket` by [@quincylvania](https://github.com/quincylvania)

Add variant icon:

- <img src="https://pinhead.ink/v14/turtle_shell_top.svg" width="15px"/> Add `turtle_shell_top` by [@quincylvania](https://github.com/quincylvania)

Add pixel icon:

- <img src="https://pinhead.ink/v14/pixel_skull.svg" width="15px"/> Add `pixel_skull` by [@quincylvania](https://github.com/quincylvania)

### Redesigned icons

- <img src="https://pinhead.ink/v13/dog_wearing_collar.svg" width="15px"/> -> <img src="https://pinhead.ink/v14/dog_wearing_collar.svg" width="15px"/> `dog_wearing_collar`
- <img src="https://pinhead.ink/v13/comb_and_dog_wearing_collar.svg" width="15px"/> -> <img src="https://pinhead.ink/v14/comb_and_dog_wearing_collar.svg" width="15px"/> `comb_and_dog_wearing_collar`
- <img src="https://pinhead.ink/v13/dog_wearing_collar_in_shelter.svg" width="15px"/> -> <img src="https://pinhead.ink/v14/dog_wearing_collar_in_shelter.svg" width="15px"/> `dog_wearing_collar_in_shelter`
- <img src="https://pinhead.ink/v13/mounted_slotted_dispenser_with_dog_wearing_collar.svg" width="15px"/> -> <img src="https://pinhead.ink/v14/mounted_slotted_dispenser_with_dog_wearing_collar.svg" width="15px"/> `mounted_slotted_dispenser_with_dog_wearing_collar`
- <img src="https://pinhead.ink/v13/file_box.svg" width="15px"/> -> <img src="https://pinhead.ink/v14/file_box.svg" width="15px"/> `file_box`

## [13.0.0] - 2026-03-07

⚠️ This major release contains new and renamed icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Renamed icons

- <img src="https://pinhead.ink/v13/digital_totem_with_apps.svg" width="15px"/> `app_terminal` -> `digital_totem_with_apps`
- <img src="https://pinhead.ink/v13/bifold_map_with_dotted_line_to_x.svg" width="15px"/> `treasure_map` -> `bifold_map_with_dotted_line_to_x`

### Added icons

Add "digital totem" icons:

- <img src="https://pinhead.ink/v13/digital_totem_with_info_i.svg" width="15px"/> Add `digital_totem_with_info_i` by [@dschep](https://github.com/dschep) ([#74](https://github.com/waysidemapping/pinhead/issues/74))
- <img src="https://pinhead.ink/v13/digital_totem.svg" width="15px"/> Add `digital_totem` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/digital_totem_with_wifi.svg" width="15px"/> Add `digital_totem_with_wifi` by [@quincylvania](https://github.com/quincylvania)

Add icons for pounds sterling sign:

- <img src="https://pinhead.ink/v13/pound.svg" width="15px"/> Add `pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/car_with_pound.svg" width="15px"/> Add `car_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/campsite_with_pound.svg" width="15px"/> Add `campsite_with_pound` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/tipi_campsite_with_pound.svg" width="15px"/> Add `tipi_campsite_with_pound` by [@quincylvania](https://github.com/quincylvania)

Integrate [princesse](https://github.com/Viglino/map-font-symbols/tree/main/princesse) and [pirate](https://github.com/Viglino/map-font-symbols/tree/main/pirate) map icons by [@Viglino](https://github.com/Viglino) (CC0):

- <img src="https://pinhead.ink/v13/castle_tower_with_battlement_and_spire_and_pennon.svg" width="15px"/> Add `castle_tower_with_battlement_and_spire_and_pennon` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_with_battlements.svg" width="15px"/> Add `castle_with_battlements` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_with_battlements_and_spires.svg" width="15px"/> Add `castle_with_battlements_and_spires` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_with_spires.svg" width="15px"/> Add `castle_with_spires` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_gate_with_battlements_and_spires.svg" width="15px"/> Add `castle_gate_with_battlements_and_spires` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_gate_with_battlements.svg" width="15px"/> Add `castle_gate_with_battlements` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/castle_with_battlements_and_turret.svg" width="15px"/> Add `castle_with_battlements_and_turret` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/star_wand_with_stardust.svg" width="15px"/> Add `star_wand_with_stardust` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/pumpkin_shaped_carriage.svg" width="15px"/> Add `pumpkin_shaped_carriage` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/heart_shaped_carriage.svg" width="15px"/> Add `heart_shaped_carriage` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/veiled_hennin_with_star.svg" width="15px"/> Add `veiled_hennin_with_star` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/wizards_hat_with_star.svg" width="15px"/> Add `wizards_hat_with_star` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/astrologers_hat.svg" width="15px"/> Add `astrologers_hat` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/pumpkin_under_stardust.svg" width="15px"/> Add `pumpkin_under_stardust` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/pumpkin.svg" width="15px"/> Add `pumpkin` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/cast_iron_key_with_heart_shaped_handle.svg" width="15px"/> Add `cast_iron_key_with_heart_shaped_handle` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/crown.svg" width="15px"/> Add `crown` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/frog_with_cartoon_eyes_and_open_mouth.svg" width="15px"/> Add `frog_with_cartoon_eyes_and_open_mouth` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/genie_lamp_with_stardust.svg" width="15px"/> Add `genie_lamp_with_stardust` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/unicorn_rearing.svg" width="15px"/> Add `unicorn_rearing` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/unicorn_head.svg" width="15px"/> Add `unicorn_head` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/winged_horse_rearing.svg" width="15px"/> Add `winged_horse_rearing` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/fancy_mirror_with_reflection_and_stars.svg" width="15px"/> Add `fancy_mirror_with_reflection_and_stars` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/butterfly_with_stars_and_dots.svg" width="15px"/> Add `butterfly_with_stars_and_dots` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/butterfly.svg" width="15px"/> Add `butterfly` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/sailing_ship_in_water.svg" width="15px"/> Add `sailing_ship_in_water` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/four_legged_octopus_with_cartoon_eyes.svg" width="15px"/> Add `four_legged_octopus_with_cartoon_eyes` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/four_legged_octopus.svg" width="15px"/> Add `four_legged_octopus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/four_legged_squid_with_cartoon_eyes.svg" width="15px"/> Add `four_legged_squid_with_cartoon_eyes` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/four_legged_squid.svg" width="15px"/> Add `four_legged_squid` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/parrot.svg" width="15px"/> Add `parrot` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/shark_dorsal_fin_in_waters.svg" width="15px"/> Add `shark_dorsal_fin_in_waters` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/cartoon_bomb_with_lit_fuse.svg" width="15px"/> Add `cartoon_bomb_with_lit_fuse` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/cartoon_cannon_with_lit_fuse.svg" width="15px"/> Add `cartoon_cannon_with_lit_fuse` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/ships_wheel.svg" width="15px"/> Add `ships_wheel` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/rolled_paper_in_bottle.svg" width="15px"/> Add `rolled_paper_in_bottle` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/rolled_paper_in_bottle_in_water.svg" width="15px"/> Add `rolled_paper_in_bottle_in_water` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/treasure_map.svg" width="15px"/> Add `treasure_map` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/treasure_map_x.svg" width="15px"/> Add `treasure_map_x` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/open_chest_with_treasure_and_sparkles.svg" width="15px"/> Add `open_chest_with_treasure_and_sparkles` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/flintlock_pistol.svg" width="15px"/> Add `flintlock_pistol` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/barrel_with_bunghole.svg" width="15px"/> Add `barrel_with_bunghole` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/spyglass.svg" width="15px"/> Add `spyglass` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/tricorne_hat_with_skull.svg" width="15px"/> Add `tricorne_hat_with_skull` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/skull_above_crossed_bones.svg" width="15px"/> Add `skull_above_crossed_bones` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/skull_above_crossed_cutlasses.svg" width="15px"/> Add `skull_above_crossed_cutlasses` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/ragged_flag_with_skull.svg" width="15px"/> Add `ragged_flag_with_skull` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/skull_rock_outline.svg" width="15px"/> Add `skull_rock_outline` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/skull_rock.svg" width="15px"/> Add `skull_rock` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v13/round_bottomed_flask.svg" width="15px"/> Add `round_bottomed_flask` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/coconut_palm_tree.svg" width="15px"/> Add `coconut_palm_tree` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))
- <img src="https://pinhead.ink/v13/coconut_palm_tree_on_hill_in_water.svg" width="15px"/> Add `coconut_palm_tree_on_hill_in_water` by [@viglino](https://github.com/viglino) ([#81](https://github.com/waysidemapping/pinhead/issues/81))


## [12.0.0] - 2026-03-06

⚠️ This major release contains new icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Distribution changes

- Pinhead icons are now synced to Wikimedia Commons ([#65](https://github.com/waysidemapping/pinhead/issues/65))

### Added icons

Add target and life ring icons. Thank you to new Pinhead contributor [@westnordost](https://github.com/westnordost)!

- <img src="https://pinhead.ink/v12/target_with_archery_arrow_at_bullseye.svg" width="15px"/> Add `target_with_archery_arrow_at_bullseye` by [@westnordost](https://github.com/westnordost) ([#67](https://github.com/waysidemapping/pinhead/issues/67))
- <img src="https://pinhead.ink/v12/target.svg" width="15px"/> Add `target` by [@westnordost](https://github.com/westnordost), [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v12/life_ring.svg" width="15px"/> Add `life_ring` by [@westnordost](https://github.com/westnordost) ([#68](https://github.com/waysidemapping/pinhead/issues/68))

Add icons of person carrying skis based on a design by new contributor [@ycouble](https://github.com/ycouble)! Thank you!

- <img src="https://pinhead.ink/v12/person_carrying_ski.svg" width="15px"/> Add `person_carrying_ski` by [@ycouble](https://github.com/ycouble), [@quincylvania](https://github.com/quincylvania) ([#69](https://github.com/waysidemapping/pinhead/issues/69))
- <img src="https://pinhead.ink/v12/person_carrying_ski_and_ski_poles.svg" width="15px"/> Add `person_carrying_ski_and_ski_poles` by [@ycouble](https://github.com/ycouble), [@quincylvania](https://github.com/quincylvania) ([#69](https://github.com/waysidemapping/pinhead/issues/69))
- <img src="https://pinhead.ink/v12/person_carrying_skis.svg" width="15px"/> Add `person_carrying_skis` by [@ycouble](https://github.com/ycouble), [@quincylvania](https://github.com/quincylvania) ([#69](https://github.com/waysidemapping/pinhead/issues/69))
- <img src="https://pinhead.ink/v12/person_carrying_skis_and_ski_poles.svg" width="15px"/> Add `person_carrying_skis_and_ski_poles` by [@ycouble](https://github.com/ycouble), [@quincylvania](https://github.com/quincylvania) ([#69](https://github.com/waysidemapping/pinhead/issues/69))

Add icons:

- <img src="https://pinhead.ink/v12/three_inch_floppy_disk.svg" width="15px"/> Add `three_inch_floppy_disk` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v12/pixel_circle_with_dot.svg" width="15px"/> Add `pixel_circle_with_dot` by [@quincylvania](https://github.com/quincylvania)

## [11.0.0] - 2026-03-05

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

Add candlepin bowling icons. Thank you to new Pinhead contributor [@petercooperjr](https://github.com/petercooperjr)!

- <img src="https://pinhead.ink/v11/candlepins.svg" width="15px"/> Add `candlepins` by [@petercooperjr](https://github.com/petercooperjr) ([#61](https://github.com/waysidemapping/pinhead/issues/61))
- <img src="https://pinhead.ink/v11/candlepin_with_ball.svg" width="15px"/> Add `candlepin_with_ball` by [@petercooperjr](https://github.com/petercooperjr) ([#61](https://github.com/waysidemapping/pinhead/issues/61))

Add other bowling icons:

- <img src="https://pinhead.ink/v11/bowling_pin.svg" width="15px"/> Add `bowling_pin` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/bowling_ball.svg" width="15px"/> Add `bowling_ball` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/pixel_bowling_ball.svg" width="15px"/> Add `pixel_bowling_ball` by [@quincylvania](https://github.com/quincylvania)

Add visitor or information center icon:

- <img src="https://pinhead.ink/v11/house_with_flag_and_info_i.svg" width="15px"/> Add `house_with_flag_and_info_i` by [@dschep](https://github.com/dschep) ([#60](https://github.com/waysidemapping/pinhead/issues/60))

Add euro symbol icons:

- <img src="https://pinhead.ink/v11/euro.svg" width="15px"/> Add `euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/car_with_euro.svg" width="15px"/> Add `car_with_euro` by [@quincylvania](https://github.com/quincylvania)

Add campsite icons:

- <img src="https://pinhead.ink/v11/campsite_with_dollar.svg" width="15px"/> Add `campsite_with_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/campsite_with_euro.svg" width="15px"/> Add `campsite_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/campsite_with_canoe.svg" width="15px"/> Add `campsite_with_canoe` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/campsites.svg" width="15px"/> Add `campsites` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v11/tipi_campsite.svg" width="15px"/> Add `tipi_campsite` by [@quincylvania](https://github.com/quincylvania) ([#52](https://github.com/waysidemapping/pinhead/issues/52))
- <img src="https://pinhead.ink/v11/tipi_campsite_with_dollar.svg" width="15px"/> Add `tipi_campsite_with_dollar` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/tipi_campsite_with_euro.svg" width="15px"/> Add `tipi_campsite_with_euro` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/tipi_campsites.svg" width="15px"/> Add `tipi_campsites` by [@quincylvania](https://github.com/quincylvania) ([#52](https://github.com/waysidemapping/pinhead/issues/52))

Add tent icons:

- <img src="https://pinhead.ink/v11/a_frame_tent.svg" width="15px"/> Add `a_frame_tent` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v11/a_frame_tents.svg" width="15px"/> Add `a_frame_tents` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v11/a_frame_sidewall_tent.svg" width="15px"/> Add `a_frame_sidewall_tent` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v11/a_frame_sidewall_tents.svg" width="15px"/> Add `a_frame_sidewall_tents` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v11/wall_tent.svg" width="15px"/> Add `wall_tent` by [@quincylvania](https://github.com/quincylvania) ([#53](https://github.com/waysidemapping/pinhead/issues/53))

Add toilet icons:

- <img src="https://pinhead.ink/v11/sitting_tank_toilet.svg" width="15px"/> Add `sitting_tank_toilet` by [@quincylvania](https://github.com/quincylvania) ([#39](https://github.com/waysidemapping/pinhead/issues/39))
- <img src="https://pinhead.ink/v11/sitting_tank_toilet_with_droplet.svg" width="15px"/> Add `sitting_tank_toilet_with_droplet` by [@quincylvania](https://github.com/quincylvania) ([#39](https://github.com/waysidemapping/pinhead/issues/39))

Add combined phones icon:

- <img src="https://pinhead.ink/v11/mobile_phone_with_keypad_and_antenna_beside_mobile_phone_with_touchscreen_and_antenna.svg" width="15px"/> Add `mobile_phone_with_keypad_and_antenna_beside_mobile_phone_with_touchscreen_and_antenna` by [@quincylvania](https://github.com/quincylvania)

Add gender and sexuality icons:

- <img src="https://pinhead.ink/v11/mars.svg" width="15px"/> Add `mars` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/venus_mars.svg" width="15px"/> Add `venus_mars` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/venus_with_mars.svg" width="15px"/> Add `venus_with_mars` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/double_venus.svg" width="15px"/> Add `double_venus` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/double_mars.svg" width="15px"/> Add `double_mars` by [@quincylvania](https://github.com/quincylvania)

Add pixel icons:

- <img src="https://pinhead.ink/v11/pixel_map_pin.svg" width="15px"/> Add `pixel_map_pin` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v11/pixel_map_pin_with_dot.svg" width="15px"/> Add `pixel_map_pin_with_dot` by [@quincylvania](https://github.com/quincylvania)

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v10/tents.svg" width="15px"/> `tents` -> <img src="https://pinhead.ink/v11/wall_tents.svg" width="15px"/> `wall_tents` ([#53](https://github.com/waysidemapping/pinhead/issues/53))

### Redesigned icons

- <img src="https://pinhead.ink/v10/bowling_pins.svg" width="15px"/> -> <img src="https://pinhead.ink/v11/bowling_pins.svg" width="15px"/> `bowling_pins` ([#52](https://github.com/waysidemapping/pinhead/issues/52))
- <img src="https://pinhead.ink/v10/bowling_pin_and_bowling_ball.svg" width="15px"/> -> <img src="https://pinhead.ink/v11/bowling_pin_and_bowling_ball.svg" width="15px"/> `bowling_pin_and_bowling_ball` ([#52](https://github.com/waysidemapping/pinhead/issues/52))
- <img src="https://pinhead.ink/v10/campsite.svg" width="15px"/> -> <img src="https://pinhead.ink/v11/campsite.svg" width="15px"/> `campsite` ([#53](https://github.com/waysidemapping/pinhead/issues/53))
- <img src="https://pinhead.ink/v10/venus.svg" width="15px"/> -> <img src="https://pinhead.ink/v11/venus.svg" width="15px"/> `venus`

## [10.0.0] - 2026-03-03

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

Add bicycle icons. Many thanks to Pinhead's first outside contributor [@dschep](https://github.com/dschep)!

- <img src="https://pinhead.ink/v10/person_riding_bicycle_up_uneven_slope.svg" width="15px"/> Add `person_riding_bicycle_up_uneven_slope` imported by [@dschep](https://github.com/dschep)
- <img src="https://pinhead.ink/v10/person_riding_bicycle_down_uneven_slope.svg" width="15px"/> Add `person_riding_bicycle_down_uneven_slope` by [@dschep](https://github.com/dschep)
- <img src="https://pinhead.ink/v10/cargobike.svg" width="15px"/> Add `cargobike` designed by [@dschep](https://github.com/dschep)
- <img src="https://pinhead.ink/v10/cargobike_on_parking_line.svg" width="15px"/> Add `cargobike_on_parking_line` designed by [@dschep](https://github.com/dschep)
- <img src="https://pinhead.ink/v10/cargobike_in_parking_structure.svg" width="15px"/> Add `cargobike_in_parking_structure` designed by [@dschep](https://github.com/dschep)

Add various other icons:

- <img src="https://pinhead.ink/v10/flat_head_thumb_tack.svg" width="15px"/> Add `flat_head_thumb_tack` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/flag.svg" width="15px"/> Add `flag`
- <img src="https://pinhead.ink/v10/flagstick_with_pennant.svg" width="15px"/> Add `flagstick_with_pennant` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/flagstick_with_pennant_in_hole.svg" width="15px"/> Add `flagstick_with_pennant_in_hole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/flagstick_with_flag.svg" width="15px"/> Add `flagstick_with_flag` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/flagstick_with_flag_in_hole.svg" width="15px"/> Add `flagstick_with_flag_in_hole` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/waterfall_into_water.svg" width="15px"/> Add `waterfall_into_water`
- <img src="https://pinhead.ink/v10/waterfall.svg" width="15px"/> Add `waterfall`
- <img src="https://pinhead.ink/v10/person_climbing.svg" width="15px"/> Add `person_climbing`
- <img src="https://pinhead.ink/v10/bus_within_guideway.svg" width="15px"/> Add `bus_within_guideway` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/bus_with_pantograph.svg" width="15px"/> Add `bus_with_pantograph` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/shopping_bag_with_heart.svg" width="15px"/> Add `shopping_bag_with_heart` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/shopping_bag_with_ampersand.svg" width="15px"/> Add `shopping_bag_with_ampersand` by [@quincylvania](https://github.com/quincylvania)
- <img src="https://pinhead.ink/v10/music_notes_eighth.svg" width="15px"/> Add `music_notes_eighth`
- <img src="https://pinhead.ink/v10/pixel_anchor.svg" width="15px"/> Add `pixel_anchor` by [@quincylvania](https://github.com/quincylvania)

### Redesigned icons

- <img src="https://pinhead.ink/v9/ticket_in_slot.svg" width="15px"/> -> <img src="https://pinhead.ink/v10/ticket_in_slot.svg" width="15px"/> `ticket_in_slot`

### Renamed icons

- <img src="https://pinhead.ink/v10/flagpole_with_flag.svg" width="15px"/> `flag` -> `flagpole_with_flag`
- <img src="https://pinhead.ink/v10/flagstick_with_pennant_on_square.svg" width="15px"/> `pennant_on_square` -> `flagstick_with_pennant_on_square`
- <img src="https://pinhead.ink/v10/person_swinging_golf_club_beside_flagstick_with_pennant.svg" width="15px"/> `person_swinging_golf_club_beside_golf_pin` -> `person_swinging_golf_club_beside_flagstick_with_pennant`
- <img src="https://pinhead.ink/v10/waterfall_with_froth.svg" width="15px"/> `waterfall` -> `waterfall_with_froth`

## [9.0.0] - 2026-03-01

⚠️ This major release contains new icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

Add sugar-related icons:

- <img src="https://pinhead.ink/v9/sugar_cubes.svg" width="15px"/> Add `sugar_cubes`
- <img src="https://pinhead.ink/v9/sugarcane_stalk_with_leaves.svg" width="15px"/> Add `sugarcane_stalk_with_leaves`
- <img src="https://pinhead.ink/v9/sugarcane_stalk_with_top_leaves.svg" width="15px"/> Add `sugarcane_stalk_with_top_leaves`
- <img src="https://pinhead.ink/v9/sugarcane_stalks_with_top_leaves.svg" width="15px"/> Add `sugarcane_stalks_with_top_leaves`
- <img src="https://pinhead.ink/v9/syrup_jug_with_sugarcane_stalk_with_leaves.svg" width="15px"/> Add `syrup_jug_with_sugarcane_stalk_with_leaves`
- <img src="https://pinhead.ink/v9/syrup_jug_with_sugarcane_stalk_with_leaves_and_droplet.svg" width="15px"/> Add `syrup_jug_with_sugarcane_stalk_with_leaves_and_droplet`

Add icons in the pixel style:

- <img src="https://pinhead.ink/v9/pixel_conifer_tree.svg" width="15px"/> Add `pixel_conifer_tree`
- <img src="https://pinhead.ink/v9/pixel_broadleaved_tree.svg" width="15px"/> Add `pixel_broadleaved_tree`
- <img src="https://pinhead.ink/v9/pixel_apple.svg" width="15px"/> Add `pixel_apple`
- <img src="https://pinhead.ink/v9/pixel_megalith.svg" width="15px"/> Add `pixel_megalith`
- <img src="https://pinhead.ink/v9/pixel_star.svg" width="15px"/> Add `pixel_star`
- <img src="https://pinhead.ink/v9/pixel_circle.svg" width="15px"/> Add `pixel_circle`
- <img src="https://pinhead.ink/v9/pixel_circle_outline.svg" width="15px"/> Add `pixel_circle_outline`
- <img src="https://pinhead.ink/v9/pixel_circle_with_star.svg" width="15px"/> Add `pixel_circle_with_star`
- <img src="https://pinhead.ink/v9/pixel_house_with_chimney.svg" width="15px"/> Add `pixel_house_with_chimney`
- <img src="https://pinhead.ink/v9/pixel_house_with_flag.svg" width="15px"/> Add `pixel_house_with_flag`
- <img src="https://pinhead.ink/v9/pixel_classical_building.svg" width="15px"/> Add `pixel_classical_building`
- <img src="https://pinhead.ink/v9/pixel_classical_building_with_flag.svg" width="15px"/> Add `pixel_classical_building_with_flag`
- <img src="https://pinhead.ink/v9/pixel_classical_building_with_dome_and_flag.svg" width="15px"/> Add `pixel_classical_building_with_dome_and_flag`
- <img src="https://pinhead.ink/v9/pixel_dome_with_flag.svg" width="15px"/> Add `pixel_dome_with_flag`
- <img src="https://pinhead.ink/v9/pixel_plane.svg" width="15px"/> Add `pixel_plane`

## [8.0.0] - 2026-02-28

⚠️ This major release contains new icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Distribution changes

- A QGIS plugin for Pinhead is now available

### Added icons

- <img src="https://pinhead.ink/v8/syrup_jug.svg" width="15px"/> Add `syrup_jug`
- <img src="https://pinhead.ink/v8/syrup_jug_with_maple_leaf.svg" width="15px"/> Add `syrup_jug_with_maple_leaf`
- <img src="https://pinhead.ink/v8/syrup_jug_with_maple_leaf_and_droplet.svg" width="15px"/> Add `syrup_jug_with_maple_leaf_and_droplet`
- <img src="https://pinhead.ink/v8/slice_of_pan_bread.svg" width="15px"/> Add `slice_of_pan_bread`
- <img src="https://pinhead.ink/v8/slice_of_pan_bread_outline.svg" width="15px"/> Add `slice_of_pan_bread_outline`
- <img src="https://pinhead.ink/v8/ladder.svg" width="15px"/> Add `ladder`
- <img src="https://pinhead.ink/v8/step_ladder.svg" width="15px"/> Add `step_ladder`
- <img src="https://pinhead.ink/v8/step_ladder_doubled_sided.svg" width="15px"/> Add `step_ladder_doubled_sided`
- <img src="https://pinhead.ink/v8/wifi_weak_signal.svg" width="15px"/> Add `wifi_weak_signal`
- <img src="https://pinhead.ink/v8/wifi_weakest_signal.svg" width="15px"/> Add `wifi_weakest_signal`
- <img src="https://pinhead.ink/v8/wifi_no_signal.svg" width="15px"/> Add `wifi_no_signal`
- <img src="https://pinhead.ink/v8/wifi_no_signal_with_x.svg" width="15px"/> Add `wifi_no_signal_with_x`
- <img src="https://pinhead.ink/v8/phone_bars.svg" width="15px"/> Add `phone_bars`
- <img src="https://pinhead.ink/v8/phone_bars_weak_signal.svg" width="15px"/> Add `phone_bars_weak_signal`
- <img src="https://pinhead.ink/v8/phone_bars_weaker_signal.svg" width="15px"/> Add `phone_bars_weaker_signal`
- <img src="https://pinhead.ink/v8/phone_bars_weakest_signal.svg" width="15px"/> Add `phone_bars_weakest_signal`
- <img src="https://pinhead.ink/v8/phone_bars_no_signal.svg" width="15px"/> Add `phone_bars_no_signal`
- <img src="https://pinhead.ink/v8/phone_bars_no_signal_with_x.svg" width="15px"/> Add `phone_bars_no_signal_with_x`

## [7.0.0] - 2026-02-27

⚠️ This major release contains new icons that may affect your setup. A machine-readable version of this changelog can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

- <img src="https://pinhead.ink/v7/canoe_on_sedan.svg" width="15px"/> Add `canoe_on_sedan`
- <img src="https://pinhead.ink/v7/canoe_on_station_wagon.svg" width="15px"/> Add `canoe_on_station_wagon`
- <img src="https://pinhead.ink/v7/canoe_on_pickup_truck.svg" width="15px"/> Add `canoe_on_pickup_truck`
- <img src="https://pinhead.ink/v7/pickup_truck_with_truck_cap.svg" width="15px"/> Add `pickup_truck_with_truck_cap`
- <img src="https://pinhead.ink/v7/conifer_tree_with_antenna_array.svg" width="15px"/> Add `conifer_tree_with_antenna_array`
- <img src="https://pinhead.ink/v7/shed.svg" width="15px"/> Add `shed`
- <img src="https://pinhead.ink/v7/plus.svg" width="15px"/> Add `plus`
- <img src="https://pinhead.ink/v7/roman_numeral_i.svg" width="15px"/> Add `roman_numeral_i`
- <img src="https://pinhead.ink/v7/roman_numeral_ii.svg" width="15px"/> Add `roman_numeral_ii`
- <img src="https://pinhead.ink/v7/roman_numeral_iii.svg" width="15px"/> Add `roman_numeral_iii`
- <img src="https://pinhead.ink/v7/roman_numeral_iv.svg" width="15px"/> Add `roman_numeral_iv`
- <img src="https://pinhead.ink/v7/roman_numeral_v.svg" width="15px"/> Add `roman_numeral_v`
- <img src="https://pinhead.ink/v7/roman_numeral_vi.svg" width="15px"/> Add `roman_numeral_vi`
- <img src="https://pinhead.ink/v7/roman_numeral_vii.svg" width="15px"/> Add `roman_numeral_vii`
- <img src="https://pinhead.ink/v7/roman_numeral_viii.svg" width="15px"/> Add `roman_numeral_viii`
- <img src="https://pinhead.ink/v7/roman_numeral_ix.svg" width="15px"/> Add `roman_numeral_ix`
- <img src="https://pinhead.ink/v7/roman_numeral_x.svg" width="15px"/> Add `roman_numeral_x`
- <img src="https://pinhead.ink/v7/roman_numeral_xi.svg" width="15px"/> Add `roman_numeral_xi`
- <img src="https://pinhead.ink/v7/roman_numeral_xii.svg" width="15px"/> Add `roman_numeral_xii`
- <img src="https://pinhead.ink/v7/roman_numeral_xx.svg" width="15px"/> Add `roman_numeral_xx`

## [6.0.0] - 2026-02-26

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of the icon upgrade paths can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

- <img src="https://pinhead.ink/v6/fallout_shelter_symbol.svg" width="15px"/> Add `fallout_shelter_symbol`
- <img src="https://pinhead.ink/v6/circle_with_fallout_shelter_symbol.svg" width="15px"/> Add `circle_with_fallout_shelter_symbol`
- <img src="https://pinhead.ink/v6/pixel_ghost.svg" width="15px"/> Add `pixel_ghost`
- <img src="https://pinhead.ink/v6/terminal_screen_with_greater_than_prompt.svg" width="15px"/> Add `terminal_screen_with_greater_than_prompt`
- <img src="https://pinhead.ink/v6/terminal_screen_with_hash_prompt.svg" width="15px"/> Add `terminal_screen_with_hash_prompt`
- <img src="https://pinhead.ink/v6/terminal_screen_with_dollar_prompt.svg" width="15px"/> Add `terminal_screen_with_dollar_prompt`
- <img src="https://pinhead.ink/v6/terminal_screen_with_percent_prompt.svg" width="15px"/> Add `terminal_screen_with_percent_prompt`
- <img src="https://pinhead.ink/v6/rss.svg" width="15px"/> Add `rss`
- <img src="https://pinhead.ink/v6/chocolate_drop.svg" width="15px"/> Add `chocolate_drop`
- <img src="https://pinhead.ink/v6/womens_and_mens_separate_restrooms_symbol.svg" width="15px"/> Add `womens_and_mens_separate_restrooms_symbol`

### Redesigned icons

- <img src="https://pinhead.ink/v5/shopping_cart.svg" width="15px"/> -> <img src="https://pinhead.ink/v6/shopping_cart.svg" width="15px"/> `shopping_cart`
- <img src="https://pinhead.ink/v5/person_shushing.svg" width="15px"/> -> <img src="https://pinhead.ink/v6/person_shushing.svg" width="15px"/> `person_shushing`

### Renamed icons

All the icons with people have been renamed for consistency:

- <img src="https://pinhead.ink/v6/person_walking.svg" width="15px"/> `pedestrian` -> `person_walking`
- <img src="https://pinhead.ink/v6/sign_beside_person_walking.svg" width="15px"/> `sign_beside_pedestrian` -> `sign_beside_person_walking`
- <img src="https://pinhead.ink/v6/person_wearing_backpack_walking_with_hiking_pole.svg" width="15px"/> `pedestrian_wearing_backpack_holding_hiking_pole` -> `person_wearing_backpack_walking_with_hiking_pole`
- <img src="https://pinhead.ink/v6/person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_building.svg" width="15px"/> `pedestrian_wearing_backpack_holding_hiking_pole_under_roof` -> `person_wearing_backpack_walking_with_hiking_pole_in_gable_roofed_building`
- <img src="https://pinhead.ink/v6/person_walking_under_icy_eave.svg" width="15px"/> `pedestrian_under_icy_eave` -> `person_walking_under_icy_eave`
- <img src="https://pinhead.ink/v6/person_walking_with_white_cane.svg" width="15px"/> `pedestrian_using_white_cane` -> `person_walking_with_white_cane`
- <img src="https://pinhead.ink/v6/person_walking_between_walls.svg" width="15px"/> `pedestrian_between_walls` -> `person_walking_between_walls`
- <img src="https://pinhead.ink/v6/person_walking_on_crosswalk.svg" width="15px"/> `pedestrian_on_crosswalk` -> `person_walking_on_crosswalk`
- <img src="https://pinhead.ink/v6/person_holding_shopping_bags_walking.svg" width="15px"/> `pedestrian_holding_shopping_bags` -> `person_holding_shopping_bags_walking`
- <img src="https://pinhead.ink/v6/person_driving_motorboat_on_water.svg" width="15px"/> `motorboater_on_water` -> `person_driving_motorboat_on_water`
- <img src="https://pinhead.ink/v6/person_riding_bicycle.svg" width="15px"/> `bicyclist` -> `person_riding_bicycle`
- <img src="https://pinhead.ink/v6/person_riding_bicycle_on_crosswalk.svg" width="15px"/> `bicyclist_on_crosswalk` -> `person_riding_bicycle_on_crosswalk`
- <img src="https://pinhead.ink/v6/person_walking_and_person_riding_bicycle.svg" width="15px"/> `pedestrian_and_cyclist` -> `person_walking_and_person_riding_bicycle`
- <img src="https://pinhead.ink/v6/person_walking_and_person_riding_bicycle_on_crosswalk.svg" width="15px"/> `pedestrian_and_cyclist_on_crosswalk` -> `person_walking_and_person_riding_bicycle_on_crosswalk`
- <img src="https://pinhead.ink/v6/person_swimming_in_water.svg" width="15px"/> `swimmer_in_water` -> `person_swimming_in_water`
- <img src="https://pinhead.ink/v6/person_wind_surfing_on_water.svg" width="15px"/> `wind_surfer_on_water` -> `person_wind_surfing_on_water`
- <img src="https://pinhead.ink/v6/person_wearing_helmet_paddling_kayak_on_water.svg" width="15px"/> `kayaker_on_water` -> `person_wearing_helmet_paddling_kayak_on_water`
- <img src="https://pinhead.ink/v6/person_riding_pedal_boat_on_water.svg" width="15px"/> `pedal_boater_on_water` -> `person_riding_pedal_boat_on_water`
- <img src="https://pinhead.ink/v6/person_riding_jetski_on_water.svg" width="15px"/> `jet_skier_on_water` -> `person_riding_jetski_on_water`
- <img src="https://pinhead.ink/v6/person_diving_into_water.svg" width="15px"/> `diver_above_water` -> `person_diving_into_water`
- <img src="https://pinhead.ink/v6/person_tow_skiing_on_water.svg" width="15px"/> `towed_skier_on_water` -> `person_tow_skiing_on_water`
- <img src="https://pinhead.ink/v6/person_running.svg" width="15px"/> `runner` -> `person_running`
- <img src="https://pinhead.ink/v6/person_sleeping.svg" width="15px"/> `sleeper` -> `person_sleeping`
- <img src="https://pinhead.ink/v6/person_sleeping_in_shelter.svg" width="15px"/> `sleeper_in_shelter` -> `person_sleeping_in_shelter`
- <img src="https://pinhead.ink/v6/car_beside_person_sleeping_in_bed.svg" width="15px"/> `car_beside_sleeper_in_bed` -> `car_beside_person_sleeping_in_bed`
- <img src="https://pinhead.ink/v6/person_sleeping_in_bed.svg" width="15px"/> `sleeper_in_bed` -> `person_sleeping_in_bed`
- <img src="https://pinhead.ink/v6/people_sleeping_in_bunkbeds.svg" width="15px"/> `sleepers_in_bunkbeds` -> `people_sleeping_in_bunkbeds`
- <img src="https://pinhead.ink/v6/people_sleeping_in_opposing_bunkbeds.svg" width="15px"/> `sleepers_in_opposing_bunkbeds` -> `people_sleeping_in_opposing_bunkbeds`
- <img src="https://pinhead.ink/v6/person_climbing_with_climbing_rope.svg" width="15px"/> `climber_with_climbing_rope` -> `person_climbing_with_climbing_rope`
- <img src="https://pinhead.ink/v6/person_dancing_with_sparkles.svg" width="15px"/> `dancer_with_sparkles` -> `person_dancing_with_sparkles`
- <img src="https://pinhead.ink/v6/person_riding_skateboard.svg" width="15px"/> `skateboarder` -> `person_riding_skateboard`
- <img src="https://pinhead.ink/v6/person_cross_country_skiing.svg" width="15px"/> `cross_country_skier` -> `person_cross_country_skiing`
- <img src="https://pinhead.ink/v6/person_wearing_skis_riding_chairlift.svg" width="15px"/> `aerial_chairlift_with_skier` -> `person_wearing_skis_riding_chairlift`
- <img src="https://pinhead.ink/v6/person_wearing_backpack_scrambling_up_cliff.svg" width="15px"/> `mountaineer_with_backpack_climbing_cliff` -> `person_wearing_backpack_scrambling_up_cliff`
- <img src="https://pinhead.ink/v6/people_in_car.svg" width="15px"/> `car_with_driver_and_passenger` -> `people_in_car`
- <img src="https://pinhead.ink/v6/person_snowshoeing.svg" width="15px"/> `snowshoer` -> `person_snowshoeing`
- <img src="https://pinhead.ink/v6/person_snowboarding_downhill.svg" width="15px"/> `snowboarder` -> `person_snowboarding_downhill`
- <img src="https://pinhead.ink/v6/person_sledding_downhill.svg" width="15px"/> `sledder` -> `person_sledding_downhill`
- <img src="https://pinhead.ink/v6/person_ski_jumping.svg" width="15px"/> `ski_jumper` -> `person_ski_jumping`
- <img src="https://pinhead.ink/v6/person_spiking_volleyball.svg" width="15px"/> `volleyball_player` -> `person_spiking_volleyball`
- <img src="https://pinhead.ink/v6/person_playing_tennis.svg" width="15px"/> `tennis_player` -> `person_playing_tennis`
- <img src="https://pinhead.ink/v6/people_sitting_in_theater.svg" width="15px"/> `theater_with_audience` -> `people_sitting_in_theater`
- <img src="https://pinhead.ink/v6/person_playing_soccer.svg" width="15px"/> `soccer_player` -> `person_playing_soccer`
- <img src="https://pinhead.ink/v6/person_ice_skating.svg" width="15px"/> `ice_skater` -> `person_ice_skating`
- <img src="https://pinhead.ink/v6/person_inline_skating.svg" width="15px"/> `inline_skater` -> `person_inline_skating`
- <img src="https://pinhead.ink/v6/person_skiing_downhill.svg" width="15px"/> `downhill_skier` -> `person_skiing_downhill`
- <img src="https://pinhead.ink/v6/person_riding_dog_sled.svg" width="15px"/> `dog_sledder` -> `person_riding_dog_sled`
- <img src="https://pinhead.ink/v6/person_wearing_scuba_gear_diving.svg" width="15px"/> `scuba_diver` -> `person_wearing_scuba_gear_diving`
- <img src="https://pinhead.ink/v6/person_baseball_batting.svg" width="15px"/> `baseball_batter` -> `person_baseball_batting`
- <img src="https://pinhead.ink/v6/person_cricket_batting_at_cricket_ball.svg" width="15px"/> `cricket_batter` -> `person_cricket_batting_at_cricket_ball`
- <img src="https://pinhead.ink/v6/person_speaking_to_amphitheater.svg" width="15px"/> `public_speaker` -> `person_speaking_to_amphitheater`
- <img src="https://pinhead.ink/v6/person_wearing_backpack_and_headlamp_crouching.svg" width="15px"/> `spelunker` -> `person_wearing_backpack_and_headlamp_crouching`
- <img src="https://pinhead.ink/v6/person_wearing_helmet_padding_raft_on_water.svg" width="15px"/> `person_padding_raft_on_water` -> `person_wearing_helmet_padding_raft_on_water`
- <img src="https://pinhead.ink/v6/profile_of_person_in_hat_in_frame.svg" width="15px"/> `portrait_of_person_in_hat_in_frame` -> `profile_of_person_in_hat_in_frame`
- <img src="https://pinhead.ink/v6/person_swinging_golf_club.svg" width="15px"/> `golfer` -> `person_swinging_golf_club`
- <img src="https://pinhead.ink/v6/person_swinging_golf_club_beside_golf_pin.svg" width="15px"/> `golfer_and_golf_pin` -> `person_swinging_golf_club_beside_golf_pin`
- <img src="https://pinhead.ink/v6/person_swinging_golf_club_beside_windmill.svg" width="15px"/> `golfer_and_windmill` -> `person_swinging_golf_club_beside_windmill`
- <img src="https://pinhead.ink/v6/person_jockeying_racehorse.svg" width="15px"/> `horse_racer` -> `person_jockeying_racehorse`
- <img src="https://pinhead.ink/v6/person_boat_racing_in_waves.svg" width="15px"/> `boat_racer_on_water` -> `person_boat_racing_in_waves`
- <img src="https://pinhead.ink/v6/person_bicycle_racing.svg" width="15px"/> `bicycle_racer` -> `person_bicycle_racing`
- <img src="https://pinhead.ink/v6/person_wearing_helmet_riding_atv.svg" width="15px"/> `person_riding_atv` -> `person_wearing_helmet_riding_atv`
- <img src="https://pinhead.ink/v6/person_wearing_waiters_attire_holding_tray_with_wine_glass.svg" width="15px"/> `waiter_holding_tray_with_wine_glass` -> `person_wearing_waiters_attire_holding_tray_with_wine_glass`

## [5.0.0] - 2026-02-25

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of the icon upgrade paths can be found in the [`changelog.json`](/metadata/changelog.json) file.

### Added icons

- <img src="https://pinhead.ink/v5/clothes_hanger_holding_cloth.svg" width="15px"/> Add `clothes_hanger_holding_cloth`
- <img src="https://pinhead.ink/v5/badge_shield_with_star.svg" width="15px"/> Add `badge_shield_with_star`

Added icons from or inspired by [OpenStreetMap Americana](https://github.com/osm-americana/openstreetmap-americana) (CC0):

- <img src="https://pinhead.ink/v5/f22_raptor_fighter_jet.svg" width="15px"/> Add `f22_raptor_fighter_jet`
- <img src="https://pinhead.ink/v5/hospital_h.svg" width="15px"/> Add `hospital_h`
- <img src="https://pinhead.ink/v5/bus.svg" width="15px"/> Add `bus`
- <img src="https://pinhead.ink/v5/dome_with_flag.svg" width="15px"/> Add `dome_with_flag`
- <img src="https://pinhead.ink/v5/book_with_raised_cover.svg" width="15px"/> Add `book_with_raised_cover`
- <img src="https://pinhead.ink/v5/memorial_stone.svg" width="15px"/> Add `memorial_stone`
- <img src="https://pinhead.ink/v5/badge_shield.svg" width="15px"/> Add `badge_shield`
- <img src="https://pinhead.ink/v5/badge_shield_with_fire.svg" width="15px"/> Add `badge_shield_with_fire`
- <img src="https://pinhead.ink/v5/circle_outline_with_star.svg" width="15px"/> Add `circle_outline_with_star`
- <img src="https://pinhead.ink/v5/cocktail_with_straw.svg" width="15px"/> Add `cocktail_with_straw`
- <img src="https://pinhead.ink/v5/fork_crossing_knife.svg" width="15px"/> Add `fork_crossing_knife`
- <img src="https://pinhead.ink/v5/sleepers_in_opposing_bunkbeds.svg" width="15px"/> Add `sleepers_in_opposing_bunkbeds`
- <img src="https://pinhead.ink/v5/square_dot.svg" width="15px"/> Add `square_dot`
- <img src="https://pinhead.ink/v5/pennant_on_square.svg" width="15px"/> Add `pennant_on_square`
- <img src="https://pinhead.ink/v5/star_and_crescent_on_square.svg" width="15px"/> Add `star_and_crescent_on_square`
- <img src="https://pinhead.ink/v5/latin_cross_on_square.svg" width="15px"/> Add `latin_cross_on_square`
- <img src="https://pinhead.ink/v5/flaming_chalice.svg" width="15px"/> Add `flaming_chalice`
- <img src="https://pinhead.ink/v5/flaming_chalice_on_square.svg" width="15px"/> Add `flaming_chalice_on_square`
- <img src="https://pinhead.ink/v5/quaker_star_on_square.svg" width="15px"/> Add `quaker_star_on_square`
- <img src="https://pinhead.ink/v5/star_of_david.svg" width="15px"/> Add `star_of_david`
- <img src="https://pinhead.ink/v5/star_of_david_filled_outline.svg" width="15px"/> Add `star_of_david_filled_outline`
- <img src="https://pinhead.ink/v5/star_of_david_on_square.svg" width="15px"/> Add `star_of_david_on_square`
- <img src="https://pinhead.ink/v5/dharma_wheel_on_square.svg" width="15px"/> Add `dharma_wheel_on_square`
- <img src="https://pinhead.ink/v5/yin_yang_on_square.svg" width="15px"/> Add `yin_yang_on_square`
- <img src="https://pinhead.ink/v5/torii_on_square.svg" width="15px"/> Add `torii_on_square`
- <img src="https://pinhead.ink/v5/khanda_on_square.svg" width="15px"/> Add `khanda_on_square`
- <img src="https://pinhead.ink/v5/om_on_square.svg" width="15px"/> Add `om_on_square`

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v4/inscribed_memorial_stone.svg" width="15px"/> `inscribed_memorial_stone` -> <img src="https://pinhead.ink/v5/memorial_stone_with_inscription.svg" width="15px"/> `memorial_stone_with_inscription`

### Renamed icons

- <img src="https://pinhead.ink/v5/star_of_david_filled.svg" width="15px"/> `star_of_david` -> `star_of_david_filled`


## [4.0.0] - 2026-02-24

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of the icon upgrade paths can be found in the [`changelog.json`](/metadata/changelog.json) file. This update also include a breaking change for developers that relied on the `migrations.json` file.

### New icons

- <img src="https://pinhead.ink/v4/loaf_of_bread_with_steam.svg" width="15px"/> Add `loaf_of_bread_with_steam`
- <img src="https://pinhead.ink/v4/loaf_of_pan_bread.svg" width="15px"/> Add `loaf_of_pan_bread`
- <img src="https://pinhead.ink/v4/loaf_of_pan_bread_with_steam.svg" width="15px"/> Add `loaf_of_pan_bread_with_steam`
- <img src="https://pinhead.ink/v4/station_wagon.svg" width="15px"/> Add `station_wagon`
- <img src="https://pinhead.ink/v4/station_wagon_with_raised_hood.svg" width="15px"/> Add `station_wagon_with_raised_hood`
- <img src="https://pinhead.ink/v4/car_with_taxi_checkerboard.svg" width="15px"/> Add `car_with_taxi_checkerboard`
- <img src="https://pinhead.ink/v4/cabin.svg" width="15px"/> Add `cabin`

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v3/bread.svg" width="15px"/> `bread` -> <img src="https://pinhead.ink/v4/loaf_of_bread.svg" width="15px"/> `loaf_of_bread`

### Renamed icons

- <img src="https://pinhead.ink/v4/sedan.svg" width="15px"/> Rename `car_profile` -> `sedan`
- <img src="https://pinhead.ink/v4/sedan_with_raised_hood.svg" width="15px"/> Rename `car_profile_with_raised_hood` -> `sedan_with_raised_hood`
- <img src="https://pinhead.ink/v4/cabin_with_chimney.svg" width="15px"/> Rename `cabin` -> `cabin_with_chimney`

### Developer changes

- ⚠️ Rename `migrations.json` to [`changelog.json`](/metadata/changelog.json) file and alter format
  - Add contributor credit
  - Add mappings to source icon sets (Maki, Temaki, etc.)
  - Add data for v1 icons 
- Ensure that all SVGs contain one and only one closed `path` element

### Docs

- Add [pinhead.ink/coverage](https://pinhead.ink/coverage) page with visual comparison between icon libraries

## [3.0.0] - 2026-02-21

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of the icon upgrade paths can be found in the [`migrations.json`](/migrations.json) file.

### New icons

- <img src="https://pinhead.ink/v3/maple_leaf.svg" width="15px"/> Add `maple_leaf`
- <img src="https://pinhead.ink/v3/car_profile.svg" width="15px"/> Add `car_profile`
- <img src="https://pinhead.ink/v3/car_profile_with_raised_hood.svg" width="15px"/> Add `car_profile_with_raised_hood`
- <img src="https://pinhead.ink/v3/compact_box_truck.svg" width="15px"/> Add `compact_box_truck`
- <img src="https://pinhead.ink/v3/compact_box_truck_with_greek_cross.svg" width="15px"/> Add `compact_box_truck_with_greek_cross`
- <img src="https://pinhead.ink/v3/compact_box_truck_with_heavy_six_point_asterisk.svg" width="15px"/> Add `compact_box_truck_with_heavy_six_point_asterisk`
- <img src="https://pinhead.ink/v3/flatbed_truck.svg" width="15px"/> Add `flatbed_truck`
- <img src="https://pinhead.ink/v3/pickup_truck.svg" width="15px"/> Add `pickup_truck`
- <img src="https://pinhead.ink/v3/pickup_truck_with_crates.svg" width="15px"/> Add `pickup_truck_with_crates`
- <img src="https://pinhead.ink/v3/pickup_truck_with_raised_hood.svg" width="15px"/> Add `pickup_truck_with_raised_hood`
- <img src="https://pinhead.ink/v3/mobile_phone_with_keypad_and_antenna_and_wifi.svg" width="15px"/> Add `mobile_phone_with_keypad_and_antenna_and_wifi`
- <img src="https://pinhead.ink/v3/mobile_phone_with_touchscreen_and_antenna_and_wifi.svg" width="15px"/> Add `mobile_phone_with_touchscreen_and_antenna_and_wifi`

### Redesigned icons

- <img src="https://pinhead.ink/v2/wifi.svg" width="15px"/> -> <img src="https://pinhead.ink/v3/wifi.svg" width="15px"/> Update `wifi` to be simpler and bolder, and therefore more legible at smaller sizes and easier to combine with other icons

### Renamed and redesigned icons

- <img src="https://pinhead.ink/v2/truck_profile.svg" width="15px"/> `truck_profile` -> <img src="https://pinhead.ink/v3/box_truck.svg" width="15px"/> `box_truck`

## [2.1.1] - 2026-02-20

### Developer changes

- List added icons in [`migrations.json`](/migrations.json) file
- Include `migrations.json` file in the distribution

## [2.1.0] - 2026-02-20

### Developer changes

- Remove unnecessary `<?xml version="1.0" encoding="UTF-8"?>` declarations from every icon
- Remove unnecessary `version="1.1"` and `xmlns:xlink="http://www.w3.org/1999/xlink"` attributes from `<svg>` element of every icon

## [2.0.0] - 2026-02-20

⚠️ This major release contains new, redesigned, and renamed icons that may affect your setup. A machine-readable version of the icon upgrade paths can be found in the [`migrations.json`](/migrations.json) file.

### New icons

- <img src="https://pinhead.ink/v2/turtle_top.svg" width="15px"/> Add `turtle_top`
- <img src="https://pinhead.ink/v2/arrow_down_to_down_bracket.svg" width="15px"/> Add `arrow_down_to_down_bracket`
- <img src="https://pinhead.ink/v2/arrow_up_to_up_bracket.svg" width="15px"/> Add `arrow_up_to_up_bracket`
- <img src="https://pinhead.ink/v2/arrow_left_to_left_bracket.svg" width="15px"/> Add `arrow_left_to_left_bracket`

### Redesigned icons

- <img src="https://pinhead.ink/v1/arrow_right_to_right_bracket.svg" width="15px"/> -> <img src="https://pinhead.ink/v2/arrow_right_to_right_bracket.svg" width="15px"/> Update `arrow_right_to_right_bracket` thickness to match similar arrow icons

### Renamed icons

Various icons have been renamed due to issues found in the initial release. 

- <img src="https://pinhead.ink/v2/latin_cross.svg" width="15px"/> Rename `cross_latin` -> `latin_cross` for consistency with `greek_cross`
- <img src="https://pinhead.ink/v2/flower_bouquet.svg" width="15px"/> Rename `flower_boquette` -> `flower_bouquet` to fix spelling
- <img src="https://pinhead.ink/v2/plant_in_raised_planter.svg" width="15px"/> Rename `plan_in_raised_planter` -> `plant_in_raised_planter` to fix typo
- Rename various transit icons for consistency
  - <img src="https://pinhead.ink/v2/hanging_rail_transit_vehicle_with_destination_display.svg" width="15px"/> `hanging_rail_transit_vehicle` -> `hanging_rail_transit_vehicle_with_destination_display`
  - <img src="https://pinhead.ink/v2/transit_vehicle_with_destination_display.svg" width="15px"/> `local_transit_vehicle` -> `transit_vehicle_with_destination_display`
  - <img src="https://pinhead.ink/v2/monorail_transit_vehicle_with_destination_display.svg" width="15px"/> `monorail_transit_vehicle` -> `monorail_transit_vehicle_with_destination_display`
  - <img src="https://pinhead.ink/v2/person_boarding_bus_with_destination_display.svg" width="15px"/> `person_boarding_bus` -> `person_boarding_bus_with_destination_display`
  - <img src="https://pinhead.ink/v2/person_boarding_hanging_rail_transit_vehicle_with_destination_display.svg" width="15px"/> `person_boarding_hanging_rail_transit_vehicle` -> `person_boarding_hanging_rail_transit_vehicle_with_destination_display`
  - <img src="https://pinhead.ink/v2/person_boarding_transit_vehicle_with_destination_display.svg" width="15px"/> `person_boarding_local_transit_vehicle` -> `person_boarding_transit_vehicle_with_destination_display`
  - <img src="https://pinhead.ink/v2/person_boarding_monorail_transit_vehicle_with_destination_display.svg" width="15px"/> `person_boarding_monorail_transit_vehicle` -> `person_boarding_monorail_transit_vehicle_with_destination_display`

### Developer changes

- Add [`migrations.json`](/migrations.json) file

## [1.0.1] - 2026-02-20

- Add `version` property to the `index.json` and `index.complete.json` files

## [1.0.0] - 2026-02-19

_Initial release_
