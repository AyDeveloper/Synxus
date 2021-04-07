/*global  style*/
@font-face {
    src: url(/fonts/Roboto-Regular.ttf);
    font-family: roboto;
}

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    list-style-type: none;
    text-decoration: none;
    font-family: roboto;
}

/*body*/
body {
    position: relative;
    background: transparent;
    display: grid;
    grid-template-rows: auto 1fr auto;
}

/*mainHeader containing the logo and avatar*/
.mainHeader {
    height: 70px;
    width: 100vw;
    background: #fff;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
    z-index: 1;
}

/*header center*/
.headerCenter {
    width: 90%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

/*avatar*/
.avatar {
    display: grid;
    grid-template-columns: auto auto;
    grid-template-rows: auto;
    margin-top: 1rem;
}

.avatar .imgBox {
    width: 50px;
    height: 50px;
}

.avatar img {
    max-width: 100%;
    max-height: 100%;
    border-radius: 50%;
}

.avatar .arrowImg {
    border: transparent;
    background: transparent;
    color: #333;
    font-size: 1.5rem;
    margin-left: .4rem;
}

/*main container containing the dashboard and customer account*/
.mainContainer {
    width: 100%;
    height: calc(100vh - 70px - 70px);
    display:grid;
    grid-template-columns: .2fr 1fr;
}

/*dashboard*/
.dashboard {
    border-right: 2px solid whitesmoke;
    background: #fff;
    box-shadow: 0px 5px 6px rgba(0, 0, 0, 0.1);
}

.dashboard .dashUl{
    width: 100%;
}

.dashboard .dashUl li {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 1.5rem;
    cursor: pointer;
}

.dashboard .dashUl li img {
    margin-left: 4.5rem;
}

.dashboard .dashUl li a {
    color: #350c69;
    text-transform: uppercase;
    overflow: auto;
    white-space: nowrap;
    cursor: pointer;
    margin-left: 1.5rem;
    font-size: 16px;
}

.dashboard .dashUl li.active{
    background: #F9F7FD;
    border-left: 8px solid #7826e0;
}

.dashboard .dashUl li.overview a {
    color: white;
} 

.dashboard .dashUl li:first-child{
    background:#7826e0;
    color: white;
}

/*end of dashboard*/

/* biodataContainer */
.biodataContainer {
    display: grid;
    grid-template-rows: .2fr auto;
    row-gap: 1rem;
    padding: 1.5rem;
}

.biodataCnt {
    height: 107px;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background: #7826e0;
    padding: 1.5rem;
    border-radius: 18px;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.4);
}

.text {
    display: grid;
    grid-template-rows: auto auto;
    row-gap: .2rem;
}

.text h3 {
    font-size: 1.8rem;
    font-weight: 400;
    letter-spacing: .11rem;
}

.text p {
    font-size: 1.1rem;
}

.biodataOtherInfo {
    display: flex;
    flex-direction: row;
}

.biodataOtherInfoOne {
    background: #F0E8FB;
    width: 500px;
    height: 400px;
    border-radius: 15px;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
    margin-right: 2rem;
    display: grid;
    grid-template-rows: auto auto auto;
    row-gap: 3rem;
}

.form {
    width: 90%;
    margin: .2rem auto;
    display: grid;
    grid-template-rows: auto auto auto;
    row-gap: 1.5rem;
    padding: 1.5rem;
}

.form1 label, .form2 label {
    font-size: 1.1rem;
    color: #350c69;
}

.form1 label div, .form2 label div {
    display: grid;
    grid-template-columns: auto auto;
    column-gap: 1rem;
    grid-template-rows: auto;
    margin-top: .5rem;
}

.form1 label input, .form2 label input {
    width: 100%;
    padding: 1rem;
    outline: none;
    border: 1px solid darkgray;
}

.form1 label input.test, .form2 label input.submit {
    background: #7826e0;
    color: #fff;
    font-size: 1.1rem;
    border: transparent;
    cursor: pointer;
}

input[type=file]::file-selector-button {
    border: 2px solid #6c5ce7;
    padding: .2em .4em;
    border-radius: .2em;
    background-color: #a29bfe;
    transition: 1s;
}

.details {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}

.details p {
    margin-left: .5rem;
    color: #7826e0;
    opacity: .4;
    text-align: justify;
}

/* end of biodataOtherInfoOne*/

/* end of biodata container*/

/*main Footer*/
.mainFooter {
    position: relative;
    height: 70px;
    width: 100%;
    background: white;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
    display: flex;
    flex-direction: column;
    justify-content: center;
}

/*footerCnt*/
.footerCnt {
    width: 90%;
    margin: .2rem auto;
    display: grid;
    grid-template-columns: auto .8fr auto;
    grid-template-rows: auto;
    padding: .4rem .4rem;
    font-size: 1.2rem;
}

.copyRight p {
   color: #333;
}

.footerLinks ul {
    display: grid;
    grid-template-columns: auto auto auto auto;
    column-gap: 2rem;
    grid-template-rows: auto;
    align-items: center;
    justify-content: center;
}

.footerLinks ul li a {
    color: #333;
}

/*footer social link*/
.footerSocialLinks {
    display: grid;
    grid-template-columns: auto auto auto auto;
    column-gap: .5rem;
    grid-template-rows: auto;
}

/*End of Footer*/


