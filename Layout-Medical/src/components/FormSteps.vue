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
                        <!--
                        <div class="row">
			<div class="col-lg-6 col-md-8 col-sm-12">
				<form id="frm-teste">
                <hr>
				<label>Estados</label><select name="estado" class="form-control"><option name="cidade" disabled=""
                 selected="selected">Selecione um estado!</option><option value="0">Acre</option><option value="1">Alagoas</option><option value="2">Amazonas</option><option value="3">Amapá</option><option value="4">Bahia</option><option value="5">Ceará</option><option value="6">Distrito Federal</option><option value="7">Espírito Santo</option><option value="8">Goiás</option><option value="9">Maranhão</option><option value="10">Minas Gerais</option><option value="11">Mato Grosso do Sul</option><option value="12">Mato Grosso</option><option value="13">Pará</option><option value="14">Paraíba</option><option value="15">Pernambuco</option><option value="16">Piauí</option><option value="17">Paraná</option><option value="18">Rio de Janeiro</option><option value="19">Rio Grande do Norte</option><option value="20">Rondônia</option><option value="21">Roraima</option><option value="22">Rio Grande do Sul</option><option value="23">Santa Catarina</option><option value="24">
                 Sergipe</option><option value="25">São Paulo</option><option value="26">Tocantins</option></select><label>
                 Cidades</label><select class="form-control"></select></form>
			</div>
			<div class="clearfix"></div>
		    </div>
               <hr>-->
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
