# Calculator
Create basic Calculator with the help of Html, Css in Apache NetBeans.

//Html Code Here!
<div class="container">
            <div class="calculator">
                <form>
                    <div class="display">
                        <input type="text" name="display">
                    </div>
                    <div>
                        <input type="button" value="Calc.">
                        <input type="button" value="AC" onclick="display.value = '' ">
                        <input type="button" value="Dl" onclick="display.value = display.value.toString().slice(0,-1)">
                        <input type="button" value="/" onclick="display.value += '/' ">
                    </div>
                     <div>
                        <input type="button" value="7" onclick="display.value += '7' ">
                        <input type="button" value="8" onclick="display.value += '8' ">
                        <input type="button" value="9" onclick="display.value += '9' ">
                        <input type="button" value="*" onclick="display.value += '*' ">
                    </div>
                     <div>
                        <input type="button" value="4" onclick="display.value += '4' ">
                        <input type="button" value="5" onclick="display.value += '5' ">
                        <input type="button" value="6" onclick="display.value += '6' ">
                        <input type="button" value="-" onclick="display.value += '-' ">
                    </div>
                     <div>
                        <input type="button" value="1" onclick="display.value += '1' ">
                        <input type="button" value="2" onclick="display.value += '2' ">
                        <input type="button" value="3" onclick="display.value += '3' ">
                        <input type="button" value="+" onclick="display.value += '+' ">
                    </div>
                     <div>
                        <input type="button" value="00" onclick="display.value += '00' ">
                        <input type="button" value="0" onclick="display.value += '0' ">
                        <input type="button" value="=" onclick="display.value = eval(display.value)">
                        <input type="button" value="." onclick="display.value += '.' ">
                    </div>
                </form>
            </div>
        </div>
              
        //Css Code Here!      
        *{
    margin: 0;
    padding: 0;
    font-family: 'var','sans-serif';
    box-sizing: border-box;
}

.container{
    width:100%;
    height:100vh;
    background-color: bisque;
    display: flex;
    align-items: center;
    justify-content: center;
}

.calculator{
    background-color: yellowgreen;
    padding: 20px;
    border-radius: 11px;
}

.calculator form input{
    border: 0;
    outline: 0;
    width: 60px;
    height: 60px;
    border-radius: 10px;
    box-shadow: -9px -9px 16px rgba(256, 256, 255,0.2), 6px 6px 16px rgba(0, 0, 0,0.3);
    background: transparent;
    font-size: 20px;
    color: black;
    cursor: pointer;
    margin: 10px;
}

form .display{
    display: flex;
    justify-content: flex-end;
    margin: 20px 0;
}

form .display input{
    text-align: left;
    flex: 1;
    font-size: 45px;
    box-shadow: none;
}
