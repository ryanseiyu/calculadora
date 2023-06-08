<script setup>
    const props = defineProps(['numero1','numero2','operacao','editaNumero1','editaNumero2']);
</script>

<template>
    <form>
        <div class="row">
            <div class="col-12 d-flex justify-content-center" style="margin-bottom: 16px;">
                <div class="col-md-2" style="margin-right: 16px; width: 156px">
                    <input :value="props.numero1" @change="props.editaNumero1" required
                        type="number" placeholder="Digite o número" class="form-control" />
                </div>
                <div class="col-md-2" style="width: 156px;">
                    <input :value="props.numero2" @change="props.editaNumero2" required
                        type="number" placeholder="Digite o número" class="form-control" />
                </div>
                <div class="col-md-2" style="margin-left: 16px; width: 156px;">
                    <select @change="operacao" class="form-control"
                        style="background-color: #rgb(floralwhite); color: black;">
                        <option value="soma" style="text-align: justify; position: relative ; left:50px;">Somar</option>
                        <option value="subtracao">Subtrair</option>
                        <option value="multiplicacao">Multiplicar</option>
                        <option value="divisao">Dividir</option>
                    </select>
                </div>
            </div>
        </div>
    </form>
</template>

