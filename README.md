

## Cooking with Higher Order Functions in Clojure

Requirements:

- [ ] Emoji render in code blocks
- [ ] Emoji render in Typora markdown
- [ ] Emoji render in GitHub markdown

### the `map` function

```clojure
;; coded in emoji
(map 🔥 [🐮 🥔 🐔 🌽 🐷 🦐])
;; => [🍔 🍟 🍗 🍿 🥓 🍤]

;; now written out using words
(map cook [:cow: :potato: :chicken: :corn: :pig: :shrimp:])
;; => :hamburger: :fries: :poultry_leg: :popcorn: :bacon: :fried_shrimp:
```

### the `filter` function

```clojure
(filter vegetarian? [🍔 🍟 🍗 🍿 🥓 🍤 🥗])
;; => [🍟 🍿 🥗] ;; assuming no lard or butter were used

;; now written out using words
(filter vegetarian? [:hamburger: :fries: :poultry_leg: :popcorn: :bacon: :fried_shrimp: :green_salad])
;; => [:fries: :popcorn: :green_salad:]
```

### reduce

```clojure
(reduce eat [🍔 🍟 🍗 🍿 🥓 🍤 🥗])
;; => 💩

;; now written out using words
(reduce eat [:hamburger: :fries: :poultry_leg: :popcorn: :bacon: :fried_shrimp: :green_salad:])
;; => :poop:
```

### apply, etc..

🍞 🍪 🐟 🦑 🍖 🥚 🐣 ⏰ 🎣 🍤 🦐 🧀 🍕 🥛  `:bread: :cookie: :fish: :squid: :meat_on_bone: :egg: :hatching_chick: :alarm_clock:  :fishing_pole_and_fish: :fried_shrimp: :shrimp: :cheese: :pizza: :milk_glass:`  

🌾  `:ear_of_rice:` :rooster: :mushroom: :yum: :electric_plug: :bulb: :bee: :honey_pot: :hourglass: :watch: :ocean: :knife: :baby: :man:  :older_man:  :skull: :robot: :baby_chick: :chicken: :horse: :horse_racing: :zap: :cloud_with_rain: :open_umbrella: :sweat_drops: :sweat: :thermometer: :poop: 

:rice:  :fish:  ==> 🍣  `:rice: :fish: :sushi:`

:egg: + cook = :fried_egg:

🥒  🍅 🥕 ==>  🥗  `:cucumber: :tomato: :carrot: :green_salad:`

💐  <== 🌹 🌷 🌺  🌼     `:bouquet: :rose: :tulip: :hibiscus: :blossom:` 

Unofficially supported emoji
🧂  🥬   👨‍🍳   🥩 🥪 🥦 `:salt: :leafy_green: :male_cook: :cut_of_meat: :sandwich: :broccoli:` 

Note: These are not available yet: Butter, wood, falafel, ice, axe, razor. 

https://emojiguide.org/butter https://emojiguide.org/wood

Ideas

- fantasy? 🧙 🧛 🧞 🧚 🐉 🦄

- human? 👻 🧟 🤖 👽

- body-part? 🦵 👃 👄 🦶 👂 👁️

- animal? :dog: :cat: :rabbit: :mouse: :turtle: :snake: :lizard: :fish: 🐸 🐦 🐎 🐊 🐻  🦁 🐙

- bird? :turkey: :eagle: :chicken: :owl:

- insect? 🐜 🦋 🐛 🦗 🐞 🐝 🦟 🦂 🕷️

- dinosaur? 🦕 🦖

- fruit?  🍉 🍓 🥝 🍑

- sport? :soccer: :baseball: :football: :basketball: :bowling: :golf:

- musical-instrument? :violin: :trumpet: :musical_keyboard: :guitar: :drum:

- place? :mountain: :ocean: :desert: :volcano: 🏞️

- transportation? :bus: :train: :airplane: :car: :bike:

- furniture? 

- 🌕 moon cycle with time 🌙 🌓 🌗 🌑 🌘 🌖 🌒 🌔

- increase-age 👶 🧒 🧑 🧓 baby, child, person, older person

  ​	or :egg: :hatching_chick: :hatched_chick: :chicken:

- combine :houses: :house: 🏘️ 🏠

- apply-time 🌱 🌳 or ⏳⌛ 

- apply-heat  :thermometer: :candle: 💣 💥 🧨

- apply-wind :trumpet: :wind_face: :musical_note:

- apply-electricity :battery: :electric_plug: :zap:

- apply-magnetism ... magnet isn't yet well supported

- apply-key :key: :lock: :unlock:

- apply-axe :evergreen_tree: ... missing wood though

- apply-vaccine :syringe: :mask:

- apply-medicine :pill: 🤒 🤢

- apply-razor  🧔 🦲 🧑 ✂️ 💇 ... missing razor though

- apply-shower :shower: 

- apply-sleep :sleepy: :bed: :slightly_smiling_face:

- apply-school 🏫🎓

- apply-fire-extinguisher 🧯 :fire_extinguisher:

- apply-cold :snowflake: 🥶 

- apply-light :rainbow: :sunny: :sun_behind_rain_cloud: 🔦

More ideas:

- ⚰️ coffin as home for dead or sleeping place for vampires
- 🦴 bone as smallest irreducible part of skeleton... those there is no skeleton emoji just yet, just a skull: 💀
- Building construction with :building_construction: :construction_worker: :office:
- Homes for certain animals, insects, etc.: 🕸️ 
- Superhero quotes: Is it a 🐦​ :bird: is it a :airplane: ✈️ no, it's 🦸
- Science related transformations: ☢️ 🧲  🧬 🔭 🌌 👨‍🚀
- Something having to do with transforming sight :eye: :microscope: :telescope: ☄️ 🌠
- ... or transforming sound: :microphone: :mega: :speaking_head: 
- 