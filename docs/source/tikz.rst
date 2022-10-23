
  \node [draw, cylinder, cylinder uses custom fill, cylinder body fill=magenta!20,
  cylinder end fill=magenta!40,  shape aspect=4, rotate=90, minimum height=6cm, minimum
  width=4cm] (c) {};
  \node at (0, -1) [draw, cylinder, cylinder uses custom fill, cylinder body fill=cyan!20,
  cylinder end fill=cyan!20,  shape aspect=4, rotate=90, minimum height=4cm, minimum
  width=4cm] (d) {};
  \draw [dashed] (-2,-2.2) arc (180:360:2 and -0.5);
  \node[circle,draw, fill=cyan!40] (e) at (0.5,-2.45){};
  \coordinate(htop) at ($(c.before top)!-1*.1!(c.after top)$);
  \coordinate(hbot) at ($(c.after bottom)!-1*.1!(c.before bottom)$);
  \coordinate(hlabel) at ($(htop)!.5!(hbot)+(c.north)!.9!(c.center)$);
  \draw[|-|] (hbot)--(htop);
  \path (hlabel) node[left] {$h_0$}; %Modify height label here
  \coordinate (center) at ($(c.before top)!0.5!(c.after top)$);
  \filldraw (center) circle (1pt);
  \coordinate (rlabel) at ($(center) !0.5!(c.after top)$);
  \coordinate (rtop) at ($(center)!-1*.1!(c.after top)$);
  \coordinate (rend) at ($(c.mid east)!0.5!(c.after top)$);
  \draw[-, shorten >=-10] (center) -- (rend);
  \path (rend) node[outer sep = 10pt, left] {$r$};
