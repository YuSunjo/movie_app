function Food({name, rating}){
  return <div>
    <h2>i like {name}</h2>
    <h4>{rating}</h4>
  </div>
}
// Food.PropTypes ={
//   name: PropTypes.string.isRequired,
//   rating: PropTypes.number.isRequired,
// };

const foodILike =[ {
  id:1,
  name: 'gimchi',
  rating: 4.5,
  
},{
  id:2,
  name: 'ramen',
  rating: 4.2,
 
}
];


 {foodILike.map(dish => (
        <Food key={dish.id} name={dish.name} rating={dish.rating} />
      ))}


// add = () => {
  //   console.log('add');
  //   this.setState( (prevState) => ( {
  //     count : prevState.count+1,
  //   })
  //   )
  // }
  add = () => {
    this.setState( (prevState) => {
      return {
        count: prevState.count+1,
      }
    })
  }