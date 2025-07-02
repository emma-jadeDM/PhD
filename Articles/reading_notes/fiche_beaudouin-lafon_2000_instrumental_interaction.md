# Instrumental Interaction: An Interaction Model for Designing Post-WIP User Interfaces (Beaudouin-Lafon, 2000)

## Related work/context

Instrumental interaction is an *interaction model* extending direct manipulation. When limiting themselves to direct manipulation, it can be hard for designers to develop new interaction techniques.

**An interaction model** is a set of principles/rules/propreties as design guidelines. It describes how to combine interaction techniques in a meaningful/consistent way. It defines the "look and feel" of interaction for the users' perspective.

**An interaction model** isfocused on the design of the interaction, as opposed to the **architectural model** of an interface which is focused on the developpment aspect through functionnal elements of the interface and their relationships with each other.

Instrumental interaction is a **model-based approach**: it's higher level and aims at bridging the gap between interaction and architecture models. Models can alspo be at **device-level** (e.g. role of physical objects in interaction) or **theoritical level** (e.g. Activity Theory providing a framework of analysis of interaction techniques).

## From WIMP to post-WIMP interfaces

### Evaluating WIMP interfaces through the principles of Direct Manipulation

#### Continuous Representation of Objects of Interest (OfI)

In DM, OfI should be visible at all time. WIMP makes them *accessible* att all times but not always visible. It's because of the screen space taken by many interfaces objects that are *not* OfI (toolbars, menus, dialog boxes). These interface objects act as mediators btwn the user and OfI. 

There are also more OfI than an eye can meet, such as secondary OfI that can be "hidden" in menus (e.g. text editor stylesheets). These OfI are part of a user's mental model but aren't considered as first-class objects. Thus, they're not always visible and can be hidden in the interface.

#### Physical actions on objects vs. complex syntax

Interfaces offer a **large vocabulary of commands** contrasting with **limited inputs** (keyboard & mouse). Direct manipulation fill the lack of input possibilities by multiplying interface elements like dialog boxes.

Dialog boxes are conceptually the same thing as typing in a command-line interface, which is indirect manipulation:

- typing a command
- typing a file name (selecting an OofI)
- typing an argument (filling a dialog box)
- return key (ok button)

#### Fast, incremental and reversible operations with an immediatly-apparent offect on the OfI

WIMP is neither fast nor incremental.

- **Not fast**: lots of non-semantic actions (moving windows, flipping through tabs) + inneficiency of inputting parameters as text/numeric values
- **Not incremental**: users must explicitly commit to the change to see results. If it doesn't match their expectaction, the user has to go through the cycle of all the commands all over again. (e.g. picking a font size numerically when all the user want is a visual result)

#### Layered or spiral approach to learning

It's easy to learn the basics of DM because there's a small range of interaction BUT going **from novice to expert** is hard. One has to combine shortcuts (mouse/keyboard). Shortcuts are inconsistents from one app to the other. 

### Towards a new interaction model

Creative apps already extend WIMP (considering brushed as 1st-class-objects, providing previews, hotboxes) -> it shows a transition from WIMP to post-WIMP interaction through **richer representations** as well as **powerful interaction widgets**. 

The article suggests that post-WIMP interactions require new interaction models that are:

- **Descriptive** incorporating both existing and novel applications
- **Comparative** and not prescriptive. They should provide metrics to compare them with alternative designs and not assume *a priori* what is good/bad
- **Generative** as in supporting the creation of new interaction techniques

## Intrumental Interaction

IRL, direct manipulation of OfI is often mediated by tools (pencils vs finger painting). It's the same digitally, e.g. with menus, but menus aren't really tools. Instrumental Interaction (InstIntr) is more focused on tools.

### Definitions

#### Domain objects

DO are sets of potention OfI for the user to **act/operate on** by editing their **attributes** AND manipulating them **as a whole** (e.g. moving them around).

- **Attributes**: can be values (a 3D sphere size as a number) or more complex objects (the sphere's material as a complex entity of color, texture, etc.)
    - A **complex attribute** can be an OfI. For instance, text styles or 3D materials can be domain objects in their part of the interface.

### Interaction instruments

Interaction instruments act as **mediators btw the user and domain object** by transforming a **user action** into a **command** affecting a **targeted domain object**.

For a scroll bar: user action (clickin on an arrow of the scroll bar) is transformed into a command (scrolling) affecting the targeted domain object (the document).

Interaction instruments have **reactions** for user control of their interaction on the instrument (e.g. highlightinh an arrow when it is pressed).

They provide **feedback** when a command is applied (the thumb of the scroll bar moves up or down). Domaain objects can also provide **responses** (the document moves).

An interaction instruments decomposed interaction in **two layers**:

- Btwn **user** and **instrument**:
    - physical action of the user
    - reaction of the instrument
- Btwn **instrument** and a **domain object**:
    - command sent to the domain object by the instrument
    - response of the domain object, which an instrument can transform into feedback

### Activating instruments

One can usually activate only few or one instrument at time because of the limited input possibilites. Still, screens could display a lot of instruments and an input could be multiplexed by association one physical part with different logicial parts.

An **activated instrument** is under user's control, such as long as a physical part isassociated with a logical part (a scroll bar stays active as long as the pointer is within the scrollbar/a rectangle tool stays active until another instrument is activated)

There are two types of activation:

- **Spatial activation**:
    - caused by moving the mouse (inside the instrument for exemple)
    - cost: the instrume t must be visible, takes spaces and requires user's attention
- **Temporal activation**:
    - caused by a former action, a temporally activated instruments remains in action until another instrument is activated (tradionally called a *mode*)
    - cost: the instrument requires explicit action to trigger activation , making it slower and less direct

The costs of activation suggests interest for designer to multiplex inputs (e.g. from using a mouse's thumbwheel to using an audio mixing console). It offers a large design space permitting access to more action, which could participae in reducing activation cost. 