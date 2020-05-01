## Commenting
We can comment each line by `%` symbol.

#### Document class

  - Document will be printed on a4 paper, using the 12pt default font
  - Define that we want to use the report class template
  - Other classes : article, book, letter, slides and others
  - In the preamble we define document wide rules
  - Commands start with a name [optional arguments] {required arguments}
  - `twocolumn` : 2 column pages
  - `titlepage` : `\maketitle` generates a title page
  - `legno` : Puts equation numbers on the left side
  - `flegn` : Left align equations versus center
  - `twoside` : Print on both sides of paper
  - `openright` : If two side is used chapters begin on right hand page
  - `landscape` : If listed it displays in landscape


#### Paper Types

  - `Paper type` : letterpaper (11 x 8.5 in), a4paper (29.7 x 21 cm)
  - `legalpaper` : (14 × 8.5 in), a5paper (21×14.8 cm),
  - `executivepaper` : (10.5×7.25 in), and b5paper (25×17.6 cm)


#### Change the font family to sans serif
  - `\renewcommand{\familydefault}{\sfdefault}`

#### Start the document
```
\begin{document}

.....

\end{document}
```

#### title
```
\title{\Large{\textbf{Latex Tutorial}}}
\author{By Hossein Dehghanipout}
\date{\today}
\maketitle
```

#### Custom margins
% You can define custom margins
` \usepackage[a4paper, inner=1.7cm, outer=2.7cm, top=2cm, bottom=2cm, bindingoffset=1.2cm]{geometry} `



#### Custom fonts
Use Helvetica instead of the normal sans serif font
`\usepackage[scaled=.92]{helvet}`

Others :
% `mathpazo` :  (Palatino (Roman))
% `mathptmx` : (Times (Roman))
% `avant` : (Avant Garde (Sans Serif))
% `courier` : (Courier (Typewriter))
% `chancery` : (Zapf Chancery (Roman))
% `bookman` : (Bookman (Roman) Avant Garde (Sans Serif) Courier (Typewriter))
% `newcent` : (New Century, Avant Garde, Courier)
% `charter` : (Charter (Roman))


#### Importing Pictures
% Used to include pictures
`\usepackage{graphicx}`

% Used to wrap text around pictures
`\usepackage{wrapfig}`

#### Bonus packages
% Improve justification document wide
% `\usepackage{microtype}`

% Used to create filler text
`\usepackage{blindtext}`


% Used to compact lists
`\usepackage{enumitem}`

% Used to customize the page layout of your LaTeX documents
`\usepackage{fancyhdr}`

% Improve output of math formulas
`\usepackage{amsmath}`

% Used to create an index
`\usepackage{index}`
`\makeindex`

% Create Table of Contents Here
`\tableofcontents`

% Use roman numeral page numbering
%`\pagenumbering{roman}`
% Start numbering with page 2
% `\setcounter{page}{2}`

% Draw a decorative line at the top & bottom of the page
`\renewcommand{\headrulewidth}{2pt}`
`\renewcommand{\footrulewidth}{1pt}`


`\pagestyle{fancy}`
% Clear default headers & footers
`\fancyhf{}`



  % Use different headers for even & odd pages
  % leftmark : Chapter title, number, LE - left side on even pages
  % Uppercase by default
`\fancyhead[LE]{\leftmark} `

  % rightmark : Chapter title, number, RO - right side on odd pages
  % Make lowercase
  `\fancyhead[RO]{\nouppercase{\rightmark}}`

  % Use the same footer for pages
  `\fancyfoot[LE,RO]{\thepage}`






#### Creating custom commands
% You can define your own commands
% Anytime you type \NTT\ New Think Tank will show
`\newcommand{\NTT}{New Think Tank}`

% Or, New Think Tank in bold
`\newcommand{\NTTB}{\textbf{New Think Tank}}`

% We can add styling to whatever text is passed
`\newcommand{\typew}[1]{\texttt{#1}}`
