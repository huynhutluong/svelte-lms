<div class="middle-box">
    <div class="container">
        <div class="white-box">
            <div class="wrapper">
                <div>
                    <img src="ctu-logo.png" alt="LOGO" width="100px">
                    <h2>HỆ THỐNG LMS</h2>
                    <h2>TRƯỜNG CNTT&TT</h2>
                    <b>ĐẠI HỌC CẦN THƠ</b>
                    <p>__oOo__</p>
                </div>
                <br>
                <br>
                <form action="#" class="form">
                    <input type="text" name="username" id="usr" placeholder="Tài khoản">
                    <input { type } placeholder="Mật khẩu">
                    <p><input type="checkbox" bind:checked={visible} on:click={togglePassword}>Hiển thị mật khẩu</p>
                    <div>
                        <input type="submit" value="Đăng nhập" class="btn">
                    </div>
                </form>
            </div>
        </div>
    </div>
</div>

<script>
    let visible = false;
    $: type = visible ? "text" : "password";

    function togglePassword() {
        visible = !visible;
    }
</script>

<style>
    * {
        margin: 0;
        padding: 0;
        overflow: hidden;
    }

    .middle-box {
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        min-height: calc(100vh - 1rem);
    }

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: white;
        width: 400px;
        height: 500px;
        border-radius: 10px;
        box-shadow: 5px 10px #888;
    }

    .form {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
    }

    input {
        padding: 5px;
        border: solid 1px gray;
        border-radius: 5px;
    }

    input[type=text] {
        padding-left: 10px;
    }

    input[type=password] {
        padding-left: 10px;
    }

    .form > * {
        margin-bottom: 5px;
    }

    .btn {
        margin-top: 7px;
        padding: 10px 20px;
        background-color: navy;
        color: white;
        border-color: navy;
        border-radius: 25px;
    }

    .btn:hover {
        background-color: white;
        color: navy;
        border-color: navy;
        border-radius: 25px;
    }

</style>
