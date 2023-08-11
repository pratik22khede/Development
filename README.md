- 👋 Hi, I’m @pratik22khede
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me 7000034544

<!---
pratik22khede/pratik22khede is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
        { 
        inputList.map( (x,i)=>{
          return(
          <div className="row mb-3">
             <div class="form-group col-md-4">
             <label >First Name</label>
              <input type="text"  name="firstName" class="form-control"  placeholder="Enter First Name" onChange={ e=>handleinputchange(e,i)} />
           </div>
           <div class="form-group col-md-4">
           <label >Last Name</label>
              <input type="text"  name="lastName" class="form-control"   placeholder="Enter Last Name" onChange={ e=>handleinputchange(e,i) }/>
           </div>
           <div class="form-group col-md-2 mt-4">
           {
              inputList.length!==1 &&
              <button  className="btn btn-danger mx-1" onClick={()=> handleremove(i)}>Remove</button>
           }
           { inputList.length-1===i &&
           <button  className="btn btn-success" onClick={ handleaddclick}>Add More</button>
           }
           </div>
        </div>
          );
         } )} 

           
   </div>
 </div>
</Container>
