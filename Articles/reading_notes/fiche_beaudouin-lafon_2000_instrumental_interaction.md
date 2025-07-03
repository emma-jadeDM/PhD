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

### Reification & Meta-Instruments

Reification can be the process of turning concepts into objects/new domain objects (a text attributes collection into text styles/a set of atributes into a 3D material).

There are **primary** and **secondary** OfI.

In Instrumental Interaction, **reification is also the process of turning one (or more) commands into an instrument**. For instance, the scroll bar is a reification of the scrolling command. This helps us **analyzing existing interface** within the instrumental integration model as well as **defining guidelines to design new instruments**.

With reification, instruments are both tools and potential OfI, just like in real life a pencil can be a tool (to draw) of an OfI (when it's broken, one notice its existence) on which we can use other tools/instruments (like a sharpener). **Instruments can be used on other instruments** to fix them, organize them (tool box), to tailor them (turning a power drill into a power-saw). Common digital **meta-instruments** are menus and palettes used to select commands and tools.

### Propreties of Instruments

Propreties of instruments aren't good/bad, they exist to provide guidelines to evaluate and make change when picking an interaction technique. They also allow exploring of new areas.

#### Degree of indirection

D°of indirection is a 2D/2-axis spaxe measuring the **spatial** and **temporal** offsets generated by an instrument.

- **Spatial offset**:
    - Distance btwn the logical part of an instrument and the OfI it operates on
    - A large spatial offset isn't always indesierable (e.g. light bulb & interruptor)
    - examples: handles on a square have low spatial offset, dialog boxes have high spatial offeset
- **Temporal offset**:
    - The time btwn the physical action on the instruments and the response of the object
    - Short temporal objects is desired bc it exploits the human perception-action loop
    - examples: handles are real-time, while dialog boxes only show the operation of the action once the interaction reaches closures (e.g. ok button)

Low spatial/temporal offset = direct manipulation VS high spatial/temporal offset = indirect manipulation

#### Degree of integration

D°of integration is the **ratio** btwn the **D° of freedom** of the **logical part** of an instrument and the D°of freedom captured by the **input device**. D°of integration can be used to **compare instruments** performing **similar operations**.

It derives from the notion of integral tasks, e.g. when various D°of Freedoms are controlled by a single device. This is how yoy calculate the ratio:

- scroll bar = unidimensionnal (1) and mouse is bidimensionnal (2)
    - the D°of integration is 1/2
- 3D rotation angle = tridimensionnal (3) and mouse is bidimensionnal (2)
    - the D°of integration is 3/2

When it comes to comparing, the ratio helps us understand which interaction technique is more efficient and which has additionnal activation cost. For exemple, panning over a document can be:

- 2 scroll bars (unidimensionnal instruments to reach bidimensionnal) : ratio of 1/2 -> additionnal activation cost
- a 2D panner (bidimensionnal to reach bidimensionnal) : ratio of 2/2 (= 1) -> more efficient

#### Degree of Compatibility

The D°of compatibility is the **similarity** btw the **physical action of user** on the instrument and the **response of the object**/

- **High D°ofC**: dragging an object (follows the mvt of the mouse)
- **Low D°ofC**: scrolling with a scroll bar (moving the thumb downward moves the document upward)
- **Lower D°ofC**: text inputs to edit the size of a font (input data type is different from output data type)

An output can have **different D°ofC depending on the interaction**
. Specifying the margins of a document can be done by inputing numeric values (lower D°ofC) or by using a ruler (higher D°ofC)

## Applying the model 

### Analyzing WIMP Interfaces (Descriptive aspect of the model)

As a descriptive model, intstrumental interaction allows us to map windows/icons/menus/pointers to instruments. The article gives several exemples, I'm only developping a few of them.

- **Menus and toolbars**
- **Dialog boxes** (for complex commands, high spatial and temporal indirection, small set of standard interactors resulting in a low D° of compatibility)
- **Inspectors, propriety boxes**
- **Handles** (very direct interaction with a low degree of indirection, high degree of compatibility and good degree of integration)
- **Window tiles**
- **Keybaord shortcuts/accelerator keys**
- **Drag and drop**

-> the increasing dvpment of other interaction techniques than WIMP, such as drag and drop, shows usefulness of the II model.

### Analyzing post-WIMP Interaction Techniques (Descriptive aspect of the model)

Key aspects of post-WIMP systems analyzed:

- strong coupling btwn user action & object reponse (= small temporal offset)
- insufficent adressing of the need for ability to manipulate several dimensions/several instruments at once in the context of multidimensionnal tasks like navigation or filtering
    - more dimensions require more input devices or higher D° of integration (using two hands?)

The article then analysis a few specific interactions from the state-of-art through the lense of the II model. I'm not taking note on that.

### Designing a Text Search Instrument (Generative aspect of the model)

The article shows the generative aspect of the model through the designing of a Text Search Instrument.

- **Non-instrumental version**: dialog box searches a string through the whole document and results in a sequential action of asking the user, for each occurence of the string, wether they want to replace it or not.
- **Instrumental proposal**: the instrument developped highlights every occurence of the string, which the user can replace by clicking on it. The instrument is a box containing the text, along with a tailored scroll bar showing where the occurences are (document lengght-wise) and allows the user to navigate at different speeds. 
    - The instrument provides **feedback** about the current state of search/replace by highligting all existing occurences.
    - The instrument has a **low D° of indirection** because it gets rid of the next/prvious/replace buttons in favour of directly clicking on the occurences + navigating with the scrollbar.
    - The instrument has an **improved D° of integration** going from (0/1) with a scrollbar activated only by a click on an arrow to (1/2) with a scrollbar using the vertical position of scrolling (1 input) to control the speed AND direction (2 outputs)

## Future work

- Colored Petri Nets project using the model as both a design guide and evaluation tool
- Aims for more details + limits of the model + design principles
- Making II useful for user interface designers... AND UI developpers (developping a toolkit)