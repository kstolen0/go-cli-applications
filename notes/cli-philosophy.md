# checklist for a successful cli

## build a modular system

design with standardisation in mind such that the cli can easily be composed with other applications.  
* Utilize std in and out 
* stadard errors 
* signals and exits codes.  
* Consider data output, e.g. plain text or json.

## Build for humans first

Conversastion is the main method of human-computer interaction.
* Provide possible corrections to invalid commands
* the current state in a multi-step process
* request confirmation before doing something risky
* write readable code for future devs

## Separate interfaces from engines and policies from mechanisms

allows different applications to use the same engine through interfaces or use the same mechanism with different policies.

## Keep it simple

Only add complexiy when necessary.  
Fold complexity into the data, not the logic.

## Stay small

Dont write big programs unless you have to.


## Be transparent

help users understand how to use the program.  
Provide comprehensive help texts and examples.  
Users resorting to google is an anti-pattern.

## Be robust

The program should work in a way the user expects.  
When an error occurs, explain what is happening clearly with suggestions for a resolution.

## No surprises

Keep the program intuitive by building on top of the user's existing knowledge. e.g. + should mean addition and - should mean subtraction.  
Stay consistent with pre-existing knowledge and patterns.  

## Be succinct

Dont print out unnecessary output.  
Dont be completely quiet.  

## Fail noisily

Repair what can be repaired. When the program fails, fail noisily and as soon as possible.

## Save your time

Build software to save developer's time as opposed to the machine's time.  
Write programs that generate programs.

## Build a prototype first, then optimize

get it working, then polish it.

## Build flexible programs

make the design flexible will allow the program to be used in ways unintended.

## Design for extensibility

extend the lifespan of the program by allowing protocols to be extensible.

## Be a good CLI citizen

Bring empathy to the design and peacefully coexist with the rest of the cli ecosystem.
