# CS571-Homework-04
## Question 1
Create a custom hook `useForm` that will persist the state of all form controls in a single object:
```javascript
const App = () => {
  const [formValues, handleChange] = useForm({ email: "", password: "" });

  return (
    <div>
      <input
        name="email"
        placeholder="email"
        value={formValues.email}
        onChange={handleChange}
      />
      <input
        type="password"
        name="password"
        placeholder="password"
        value={formValues.password}
        onChange={handleChange}
      />
    </div>
  );
};
```
  
