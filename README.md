# Introduction to Vahshibafghi*


< S > →  < Statement >< S > | `λ` </br>
< Statement > → < DeclareVar >`#` |< SayStatement >`#`|< AsStatement >|< LoopStatement >|< UntilStatement ></br>
< DeclareVar > → < Name >< DefineVar ></br>
< DefineVar > → `=` < Exp > | `λ`</br>
< Name > → `@`< LoD ></br>
< Letter > → `[a-z]` | `[A-Z]`</br>
< Digit > → `0` | < NonZeroDigit > </br>
< NonZeroDigit > → `[1-9]`</br>
< LoD > → < Digit > < MoreLoD > | < Letter > < MoreLoD ></br>
< MoreLoD > → < LoD > | `λ`</br>
< String > →`”`< MoreLoD >`”`</br>
< Comp2 > →  `>` | `<` | `>:` | `<:`</br>
< Comp1 > →  `::` | `\:`</br>
< Get > → `get`</br>
< Numbers > → < Integer >< FloatPossibility ></br>
< Sign >  → `+` | `-`</br>
< MathOperator > → `*` | `/` | `%`</br>
< FloatPossibility > → `.`< IntegerContinue > | `λ`</br>
< Integer > → < NonZeroDigit >< IntegerContinue > | `0`</br>
< IntegerContinue > → < Digit > < IntegerContinue > | `λ`</br>
< Exp > → < Exp2 >< Exp3 >	</br>
< Exp2 > → < Exp4 >< Exp5 ></br>
< Exp3 > → `|`< Exp > | `λ`</br>
< Exp4 > → < Exp6 >< Exp7 ></br>
< Exp5 > → `&`< Exp > | `λ`</br>
< Exp6 > → < Exp8 >< Exp9 > </br>
< Exp7 > → < Comp1 >< Exp > | `λ`</br>
< Exp8 > →< Exp10 >< Exp11 ></br>
< Exp9 > → < Comp2 >< Exp > | `λ`</br>
< Exp10 > → < Exp12 >< Exp13 ></br>
< Exp11 > → < Sign >< Exp > | `λ`</br>
< Exp12 > → < Exp14 >< Exp15 > </br>
< Exp13 > → < MathOperator >< Exp > | `λ`</br>
< Exp14 > → `!`< Exp > | < Sign >< Exp > | < Exp16 ></br>
< Exp15 > → `^`< Exp > | `λ`</br>
< Exp16 > → `(`< Exp >`)` | < Literal > </br>
< Literal > → < Name > | < String > | < Numbers >| < Get > | `true` | `false`</br>
< AsStatement > → `as` `(` < Exp > `)` `<<`  < S >  `>>` < IfnStatement > <Finaly></br>
< IfnStatement > → `ifn` `(` < Exp > `)` `<<` < S > `>>` < IfnStatement > | `λ`</br>
< Finaly > → `finaly` `<<` < S > `>>` | `λ`</br>
< LoopStatement > → `loop` < Exp > `on` < Name > `by` < StepSign > < Numbers > `<<`  < S >  `>>`</br>
< StepSign > → < Sign > | < MathOperator ></br>
< SayStatement > → `say` < Exp ></br>
< UntilStatement > → `until` `(`< Exp >`)` `<<` < S >  `>>`</br>


