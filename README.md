

## Cooking with Higher Order Functions in Clojure

Requirements:

- [ ] Emoji render in code blocks
- [ ] Emoji render in Typora markdown
- [ ] Emoji render in GitHub markdown

### the `map` function

```clojure
;; coded in emoji
(map 🔥 [🐮 🥔 🐔 🌽 🐷])
;; => [🍔 🍟 🍗 🍿 🥓]

;; now written out using words
(map cook [:cow: :potato: :chicken: :corn: :pig:])
;; => :hamburger: :fries: :poultry-leg: :popcorn: :bacon:
```

### the `filter` function

```clojure
(filter vegetarian? [🍔 🍟 🍗 🍿 🥓])
;; => [🍟 🍿] ;; assuming no lard or butter were used

```



### reduce, apply, etc..

🍞 🍪  🐟  🦑  🍖   🥚  🐣  ⏰   🎣  🍤 🦐 :cheese: :pizza:   `:bread: :cookie: :fish: :squid: :meat_on_bone: :egg: :hatching_chick: :alarm_clock:  :fishing_pole_and_fish: :fried_shrimp: :shrimp: :cheese: :pizza:`  

🌾  `:ear_of_rice:` :rooster: :mushroom: :yum: :electric_plug: :bulb: :bee: :honey_pot: :hourglass: :watch: :ocean: :knife: :baby: :man:  :older_man:  :skull: :robot: :baby_chick: :chicken: :horse: :horse_racing: :zap: :cloud_with_rain: :open_umbrella: :sweat_drops: :sweat: :thermometer:

:rice:  :fish:  ==> 🍣  `:rice: :fish: :sushi:`

🥒  🍅 ==>  🥗  `:cucumber: :tomato: :green_salad:` 

💐  <== 🌹 🌷 🌺  🌼     `:bouquet: :rose: :tulip: :hibiscus: :blossom:` 

Unofficially supported emoji
🧂  🥬   👨‍🍳   🥩 🥪 `:salt: :leafy_green: :male_cook: :cut_of_meat: :sandwich:` ​​

Note: These are not available yet: Butter, wood.

https://emojiguide.org/butter https://emojiguide.org/wood
