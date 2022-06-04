<template>
    <div class="container" style="width: 64rem; border-radius: 4rem;">

        <div row align-items-start>

            <form
                class="row gy-2 gx-3   flex justify-content-center flex-direction-row  bg-light px-5 py-5 " align-items-center
                style=" border-radius: 2rem;">




                <div class=" col-sm text-left">
                    
                    <h1>{{ msg }}</h1>
                    <H4><b>Dados do profissional </b></H4>
                    <div class="form-group ">
                        <label for="name">Nome  completo*</label>
                        <input type="text" class="form-control" id="name" placeholder="Digite o nome completo">

                    </div>

                    <div class="form-group">
                        <label for="cpf">CPF*</label>
                        <input type="text" class="form-control" placeholder="Digite um CPF" />

                    </div>
                    <div class="form-group">
                        <label for="cpf">Número do celular*</label>
                        <input type="text" class="form-control" placeholder="(00) 0 0000-0000" />

                           <label id="campo_estado"> Estado <br> <select id="estado" style="width:150px;height:25px"> </select> </label>
                         
                          <label id="campo_cidade"> Cidade<br>
                          
                     <select id="cidade" style="width:150px;height:25px"></select>
                </label>
                </div>
                </div>
                

                <div class="col-sm " style="display: flex; align-items: center;">
                    <div class="form-group d-flex p-2 justify-content-center" > 
                    <img src="../assets/desktop-pagina-1.png" alt="Ilustração da página 1" style="width: 450px;">
                    </div>
                </div>


                <div class="container " style="width: 280%; display: flex; justify-content: left;">
                    <ProgressBar />
                </div>
                <div class="container mt-2">
                    <ButtonNext />
                </div>
            </form>

        </div>
    </div>
</template>

<script>
import ButtonNext from './ButtonNext.vue';
import ProgressBar from './ProgressBar.vue'
export default {
    name: "FormSteps",
    props: {
        msg: String,
    },
    components: { ButtonNext, ProgressBar }
};
</script>
