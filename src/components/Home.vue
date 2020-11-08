<template>
<div>
    <h1><i class="fa fa-line-chart" aria-hidden="true"></i>InvestKo</h1>  
    <br>
    <div class="row">
        <div class="col-md-12">
            <h3>Features</h3>
            <li>You May Save & Load Your Data</li>
            <li>Click on 'End Day' To Begain New Day!</li>
            <li>Live Profit or Loss Status</li>
            <li>Stock Price Changes Everyday</li><br>
            <router-link to="/stocks" class="btn btn-primary btn-lg" tag="button"><i class="fa fa-bolt" aria-hidden="true"></i> Start Trading!</router-link>
        </div>
    </div>
    <hr>
    <br>
    <p><i class="fa fa-money" aria-hidden="true"></i> Your Funds: <strong>{{ funds | currency }}</strong></p>
</div>
</template>

<script>
export default {
    computed: {
        funds() {
            return this.$store.getters.funds;
        }
    }
}
</script>

