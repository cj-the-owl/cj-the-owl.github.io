<template>
    <!-- <div class="modal" id="cartModal">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h4 class="modal-title">Your Cart</h4>
                        <button type="button" class="btn btn-close" data-bs-dismiss="modal"></button>
                    </div>
                    <div id="cart-body">
                        <div id="results">
                            <h5>Total</h5>
                        </div>
                    </div>
                    <div class="modal-footer">
                      <a class="btn me-auto">Checkout Products</a>
                      <p>Total: <span id="total"></span></p>
                    </div>
                </div>
            </div>
        </div>

        <div id="cart-container">
            <div id="cart-body"></div>
        </div> -->

        <div class="modal-overlay" @click="$emit('close-modal')">
            <div class="modal" @click.stop>
                <img class="check" src="../assets/icon-check-14.jpg" alt="">
                <h6>Saved</h6>
                <p>Your stuff has been saved</p>
                <button class="btn">Go away</button>
            </div>
            <div class="close" @click="$emit('close-modal')">
                <p>X</p>
            </div>
        </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>

    .modal-overlay {
        position: fixed;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        display: flex;
        justify-content: center;
        background-color: #F5B6E1 ;
    }

    .modal {
        text-align: center;
        background-color: #E658D4;
        height: 500px;
        width: 500px;
        margin-top: 10%;
        padding: 60px;
        border-radius: 20px; 
    }

    .close {
        margin: 10% 0 16px;
        cursor: pointer;
    }

    .check {
        width: 150px;
    }

    h6 {
      font-weight: 500;
      font-size: 28px;
      margin: 20px 0;
    }

    p {
     font-size: 16px;
     margin: 20px 0;
    }

    button {
        background-color:#F5B6E1;
        width: 150px;
        height: 40px;
        color:black;
        font-size: 14px;
        border-radius: 16px;
        margin-top: 50px;
    }
    /* .modal-header, .modal-footer {
    background-color:#e89be8 !important;
}

#cart-body {
    background-color: #F5B6E1 !important;
}

.btn {
    background: transparent;
    border: 1px solid black;
    margin-left: 30px !important;
}

.btn:hover {
    background-color: #E658D4;
    color: #A129C9;
    border: 1px solid transparent;
}

/* #quantity-input {
    background-color: transparent;
} */ 
</style>