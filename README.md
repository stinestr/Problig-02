# Problig-02
Del 1

rodfirkant = rectangle(400, 300, "solid", "red")
blakors1 = rectangle(400, 40, "solid", "blue")
blakors2 = rectangle(40, 300, "solid", "blue")
hvitkors1 = rectangle(80, 300, "solid", "white")
hvitkors2 = rectangle(400, 80, "solid", "white")

fun nordiske-flagg(background, middle, top):
  frame(
    underlay-xy((rectangle(400, 300, "solid", background)), 0, 0, 
      overlay-xy((rectangle(400, 40, "solid", middle)), 0, -135, 
        overlay-xy((rectangle(40, 300, "solid", middle)), -125, 0,
          underlay-xy((rectangle(80, 300, "solid", top)), -105, 0, 
            underlay-xy((rectangle(400, 80, "solid", top)), 0, -115, empty-image))))))
end

Norge = nordiske-flagg("red", "blue", "white")
Sverige = nordiske-flagg("blue", "yellow", "yellow")
Norge
